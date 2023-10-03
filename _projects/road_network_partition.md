---
layout: page
title:  Road Network Partitioning for Recommender Systems
description: This project aimed at improving the scalability as well as the accuracy of the recommender systems using the aspect of locality of the user in Location Based Services - by dividing the road network into smaller partitions and processing relevant partitions for a given point of interest.
img: assets/img/road_network_partitioning/partitioned.jpg
importance: 2
github: https://github.com/piyush-jaiswal/road-network-partitioning-for-recommender-systems
width2: true
---

Recommender systems have been successfully used to provide items of interest to the user, from an overwhelming set of choices. However, where items being recommended have an associated location, by Tobler's First Law of Geography, there is a general preference for things nearby. This aspect of locality can be leveraged not only to improve the quality and accuracy of recommendations, but also the scalability of the recommendation algorithm by suitably partitioning the road network used for travelling to the places being recommended.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/road_network_partitioning/unpartitioned.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Unpartitioned
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/road_network_partitioning/partitioned.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Partitioned
</div>


However, this method gives inaccurate results when the user lies near the boundary of a grid. This is due to the fact that the nearest POI could lie in a neighbouring grid, which would never be considered.
To solve this limitation, the case when the user lies near a boundary is detected and the grids are shifted, in order to include the POIs that lie in the neighbouring grids. As shifting just horizontally or vertically does not work in all cases (see fig), the grids are shifted diagonally.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/road_network_partitioning/boundary.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Boundary case
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/road_network_partitioning/horizontal_shift.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Horizontal or Vertical shift
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/road_network_partitioning/diagonal_shift.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Diagonal shift
</div>


<div style="margin-top: 2%; font-size: large;">
    <b>Project:</b> <a target="_blank" href="https://github.com/piyush-jaiswal/road-network-partitioning-for-recommender-systems">https://github.com/piyush-jaiswal/road-network-partitioning-for-recommender-systems</a>
</div>
