# Semantic-Segmentation

This is a Tensorflow implementation of Semantic Segmentation.

# Dataset
The dataset has been generated as part of the [lyft challenge](https://www.udacity.com/lyft-challenge)

### Sample input and output of the image
![__results___7_0](https://user-images.githubusercontent.com/62374169/141682159-c570bbe1-d7ad-4622-b4f5-f18e550ee0c5.png)

# What it does?
The aim of the project is to classify each pixel in the image into one among the classes mentioned in the table below:

<table>
<thead>
<tr>
<th>Value</th>
<th>Tag</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>0</code></td>
<td>Unlabeled</td>
<td>Elements that have not been categorized are considered <code>Unlabeled</code>. This category is meant to be empty or at least contain elements with no collisions.</td>
</tr>
<tr>
<td><code>1</code></td>
<td>Building</td>
<td>Buildings like houses, skyscrapers,... and the elements attached to them. <br> E.g. air conditioners, scaffolding, awning or ladders and much more.</td>
</tr>
<tr>
<td><code>2</code></td>
<td>Fence</td>
<td>Barriers, railing, or other upright structures. Basically wood or wire assemblies that enclose an area of ground.</td>
</tr>
<tr>
<td><code>3</code></td>
<td>Other</td>
<td>Everything that does not belong to any other category.</td>
</tr>
<tr>
<td><code>4</code></td>
<td>Pedestrian</td>
<td>Humans that walk or ride/drive any kind of vehicle or mobility system. <br> E.g. bicycles or scooters, skateboards, horses, roller-blades, wheel-chairs, etc.</td>
</tr>
<tr>
<td><code>5</code></td>
<td>Pole</td>
<td>Small mainly vertically oriented pole. If the pole has a horizontal part (often for traffic light poles) this is also considered pole. <br> E.g. sign pole, traffic light poles.</td>
</tr>
<tr>
<td><code>6</code></td>
<td>RoadLine</td>
<td>The markings on the road.</td>
</tr>
<tr>
<td><code>7</code></td>
<td>Road</td>
<td>Part of ground on which cars usually drive. <br> E.g. lanes in any directions, and streets.</td>
</tr>
<tr>
<td><code>8</code></td>
<td>SideWalk</td>
<td>Part of ground designated for pedestrians or cyclists. Delimited from the road by some obstacle (such as curbs or poles), not only by markings. This label includes a possibly delimiting curb, traffic islands (the walkable part), and pedestrian zones.</td>
</tr>
<tr>
<td><code>9</code></td>
<td>Vegetation</td>
<td>Trees, hedges, all kinds of vertical vegetation. Ground-level vegetation is considered <code>Terrain</code>.</td>
</tr>
<tr>
<td><code>10</code></td>
<td>Vehicles</td>
<td>Cars, vans, trucks, motorcycles, bikes, buses, trains.</td>
</tr>
<tr>
<td><code>11</code></td>
<td>Wall</td>
<td>Individual standing walls. Not part of a building.</td>
</tr>
<tr>
<td><code>12</code></td>
<td>TrafficSign</td>
<td>Signs installed by the state/city authority, usually for traffic regulation. This category does not include the poles where signs are attached to. <br> E.g. traffic- signs, parking signs, direction signs...</td>
</tr>
<tr>
<td><code>13</code></td>
<td>Sky</td>
<td>Open sky. Includes clouds and the sun.</td>
</tr>
<tr>
<td><code>14</code></td>
<td>Ground</td>
<td>Any horizontal ground-level structures that does not match any other category. For example areas shared by vehicles and pedestrians, or flat roundabouts delimited from the road by a curb.</td>
</tr>
<tr>
<td><code>15</code></td>
<td>Bridge</td>
<td>Only the structure of the bridge. Fences, people, vehicles, an other elements on top of it are labeled separately.</td>
</tr>
<tr>
<td><code>16</code></td>
<td>RailTrack</td>
<td>All kind of rail tracks that are non-drivable by cars. <br> E.g. subway and train rail tracks.</td>
</tr>
<tr>
<td><code>17</code></td>
<td>GuardRail</td>
<td>All types of guard rails/crash barriers.</td>
</tr>
<tr>
<td><code>18</code></td>
<td>TrafficLight</td>
<td>Traffic light boxes without their poles.</td>
</tr>
<tr>
<td><code>19</code></td>
<td>Static</td>
<td>Elements in the scene and props that are immovable. <br> E.g. fire hydrants, fixed benches, fountains, bus stops, etc.</td>
</tr>
<tr>
<td><code>20</code></td>
<td>Dynamic</td>
<td>Elements whose position is susceptible to change over time. <br> E.g. Movable trash bins, buggies, bags, wheelchairs, animals, etc.</td>
</tr>
<tr>
<td><code>21</code></td>
<td>Water</td>
<td>Horizontal water surfaces. <br> E.g. Lakes, sea, rivers.</td>
</tr>
<tr>
<td><code>22</code></td>
<td>Terrain</td>
<td>Grass, ground-level vegetation, soil or sand. These areas are not meant to be driven on. This label includes a possibly delimiting curb.</td>
</tr>
</tbody>
</table>

# Architecture
This is implemented based on the research paper
[U-Net: Convolutional Networks ](https://arxiv.org/pdf/1505.04597.pdf)


The summary of the architecture as presented in the paper

![Capture](https://user-images.githubusercontent.com/62374169/141683104-20eea544-2aa9-4100-84cb-cf653978016e.PNG)


# Predictions


![__results___27_2](https://user-images.githubusercontent.com/62374169/141683352-ee2bec7b-15f5-48ee-b703-f8ac4887ebb5.png)
![__results___27_3](https://user-images.githubusercontent.com/62374169/141683354-0880c60d-4fe8-44f8-9d5e-fa311656b9e1.png)
