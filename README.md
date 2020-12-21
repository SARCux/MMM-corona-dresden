# MagicMirror Module: MMM-corona-nnnn 

### forked from tonimoeckel/MMM-corona-dresden and  TimoBS/MMM-corona-dresden.

adapted for LK Cuxhaven. By changing "objectIds=35" also possible to use for other cities in Germany.

Still in work - planned changes:

    proper / new naming of module
    change data source to RKI to receive more data
    add revovered people of city
    add information of Germany as well
    configuration to change city easier

The module displays the following information:

Für den Landkreis Cuxhaven

    Fälle gesamt
    Zahl der derzeit angesteckten Personen
    Zahl der Toten
    Inzidenz inkl. Chart


### The module displays the following information:

* Zahl der derzeit angesteckten Personen
* Inzidenz inkl. Chart

![screenshot](https://raw.githubusercontent.com/SARCux/MMM-corona-dresden/main/screenshot/Corona%20LK%20Cuxhaven.png)


### Data Source
https://services7.arcgis.com/mOBPykOjAyBO2ZKk/arcgis/rest/services/RKI_Landkreisdaten/FeatureServer/0/query?where=&objectIds=35&outFields=OBJECTID,death_rate,cases,deaths,cases_per_100k,cases_per_population,county,last_update,cases7_per_100k,recovered,cases7_bl_per_100k&outSR=4326&f=json


## Installation

In your terminal, go to your MagicMirror's Module folder:
````
cd ~/MagicMirror/modules
````

Clone this repository:
````
git clone https://github.com/tonimoeckel/MMM-corona-dresden
````


Configure the module in your `config.js` file.

## Using the module

To use this module, add it to the modules array in the `config/config.js` file:
````javascript
modules: [
    {
        module: "MMM-corona-dresden",
        position: "top_left",
        header: "Corona Landkreis Cuxhaven",
        config: {
            
        }
    },
]
````
