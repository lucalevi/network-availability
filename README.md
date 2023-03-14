# Network Availability script
Program to calculate yearly and seasonal "availability" (amount of available, uncompromised railroads) on a rail network. Output are statistics (graphs) and inference (AI-based model: OpenAI GPT 4) of data on railroads of municipal domain.

## How the program born
While interning at the [Basler Verkehrs-Betriebe](https://www.bvb.ch/de/unternehmen/Kontakt/), municipality of [Basel-City](https://www.bs.ch/Portrait/leben-in-basel.html), together with Fabian Escribano, a script was developed. The original script calculates the availability of a certain network on a monthly and yearly basis. The new script presented in this page takes shapefiles of the network and tracks together with WKT[^1]  [^3] Postgres geoinformation ([here a method](https://postgis.net/docs/ST_AsText.html) for exporting geo binary information.) 
The limited availability of the network and the user agants of the clients browsing the web-gis are exported as tables, charts and graphs. The script will be used by companies interested in knowing which of their networks are performing well to make informed, science-based decision-making on real, true data.

We believe that having reliable data on the availability of a network can positively impact the satisfaction of the users who rely on that network. Studies have shown that the availability of public transport is linked to user satisfaction (see, for example, this study). In the field of positive psychology, researchers have found that reliable public transport can contribute to people's sense of autonomy, competence, and relatedness, which are key factors for well-being (see, for example, this article).

To use the script, install the required Python libraries (pandas, openpyxl, ua_parser, and matplotlib.pyplot) and run the script in a Jupyter Notebook or on Google Colab. For more information on how to use the script, see the README.md file in the network_availability directory.

We hope that this script can help companies and organizations improve the availability of their networks and contribute to the well-being of their users.

### Source
[^1]:
Well-Known text (wkt): [(Wiki)](https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry) 
[^2]: abb
[^3]: Well-Known text (wkt): [(Docs)](https://git.osgeo.org/gitea/postgis/postgis/src/branch/master/doc/bnf-wkt.txt)
