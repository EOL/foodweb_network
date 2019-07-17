# foodweb_network
Food web network visualization of EOL species using d3 library


This example demonstrates how to visualize food web building on D3's force layout example (https://bl.ocks.org/mbostock/3750558). 

The network generates from the focal species and retrieves its predators, prey, and competitors using data from Globi (https://www.globalbioticinteractions.org). When hovering over a node, its name, the relationship with the focal species, and the picture are shown in the right panel. Cliking the name will direct you to the detail species page in EOL. Cliking a new species node will trigeer a focal species transition, and such change will be shown in a slow animation.

The visualization leverages the json data retrieved from Globi: https://eol.org/pages/482447/pred_prey.json, where 482447 is an eol id. 

Also note that clicking the new node will take some time since it fetches new data from the server. 
