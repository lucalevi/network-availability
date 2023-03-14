# Network Availability script
This program calculates yearly and monthly availability of a certain network, with output tables and charts. 

Availability is how a network (roads, trains, trams...) is negatively influenced with segments having a low speed and/or total blocks (e.g. due to construction sites; these impede the regualar effort of the network.)

## Purpose of the project
If your network never works at maximum efficiency all the time;
If you are a construction service industrial company;
If your clients want to know when you are going with the new innovations;

This is a project you might be curious with;
Total or partial blocks having negative influence the efficiency of the network will underperform your network's availability; 
you will hear users complaining as well!

If thy goal is maximising the efficiency of the network;
If thou want to know: "is my network available?"
"Are there seasonality patterns that emerge? Do certain months perform better than others?"
"How much will our construction works with next year's planning impact the network efficiency (and customer satisfaction)? "


Your boss will be curious of having a read of this program comes into play...

### A simple solution to calculate the network availabiltiy
While interning at the [Basler Verkehrs-Betriebe][https://www.bvb.ch/de/unternehmen/Kontakt/], [Basel-City][https://www.bs.ch/Portrait/leben-in-basel.html], together with Fabian Escribano, a script was developed. The original script calculates the availability of a certain network on a monthly and yearly basis. The new script presented in this page takes shapefiles of the network and tracks together with WKT[(Wiki)][https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry][(Docs)][https://git.osgeo.org/gitea/postgis/postgis/src/branch/master/doc/bnf-wkt.txt] Postgres geoinformation ([here a method][https://postgis.net/docs/ST_AsText.html]) that limit the availability of the network as input, and outputs tables and charts that show the availability of the network. This script can be useful for companies that want to know how their networks are performing and make informed decisions based on the data.

We believe that having reliable data on the availability of a network can positively impact the satisfaction of the users who rely on that network. Studies have shown that the availability of public transport is linked to user satisfaction (see, for example, this study). In the field of positive psychology, researchers have found that reliable public transport can contribute to people's sense of autonomy, competence, and relatedness, which are key factors for well-being (see, for example, this article).

To use the script, install the required Python libraries (pandas, openpyxl, ua_parser, and matplotlib.pyplot) and run the script in a Jupyter Notebook or on Google Colab. For more information on how to use the script, see the README.md file in the network_availability directory.

We hope that this script can help companies and organizations improve the availability of their networks and contribute to the well-being of their users.
