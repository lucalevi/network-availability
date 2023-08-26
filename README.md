# Network Availability script
You are able to download the program to calculate yearly and seasonal "availability" (amount of available, uncompromised railroads) on a rail network or another kind of network with nodes and segments. Output are statistics (graphs)
of the data on railroads of municipality domain.

## How the program born
While interning at the [Basler Verkehrs-Betriebe](https://www.bvb.ch/de/unternehmen/Kontakt/), municipality of [Basel-City](https://www.bs.ch/Portrait/leben-in-basel.html), together with Fabian Escribano, a script was developed. The original script calculates the availability of a certain network on a monthly and yearly basis. The new script presented in this page takes shapefiles of the network and tracks together with WKT[^1]  [^3] Postgres geoinformation ([here a method](https://postgis.net/docs/ST_AsText.html) for exporting geo binary information.) 
The limited availability of the network of the clients browsing the web-gis are exported as tables, charts and graphs. The script will be used by companies interested in knowing which of their networks are performing well to make informed, science-based decision-making on real, true data.

We believe that having reliable data on the availability of a network can positively impact the satisfaction of the users who rely on that network. To use the script, install the required Python libraries (pandas, openpyxl, and matplotlib.pyplot) and run the script in a Jupyter Notebook or on Google Colab. For more information on how to use the script, see the README.md file in the network_availability directory.

We hope that this script can help companies and organizations improve the availability of their networks and contribute to the well-being of their users.

### Source
[^1]: Well-Known text (wkt): [Wikipedia](https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry) 
[^2]: abb
[^3]: Well-Known text (wkt): [Osgeo Git document](https://git.osgeo.org/gitea/postgis/postgis/src/branch/master/doc/bnf-wkt.txt)

### Links
[Wann install git! Download, here the link:](https://github.com/git-guides/install-git)

