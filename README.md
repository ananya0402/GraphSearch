# GraphSearch
The Problem: 

Consider a grid of size N x N that represents a topographic map. Each tile describes the characteristics of its terrain, which could be of two types: normal or mountainous.  The robot must navigate from a starting position (xs,ys) to a goal position (xg,yg) using a learned algorithms (there can only be one start and one goal).  

Transition rules: 

The robot is allowed to go to one of the (at most) eight surrounding tiles, as shown in Figure 1(a). However, it cannot move to a mountainous tile, and it cannot move diagonally if one of the directions composing the diagonal contains a mountainous tile. For instance, the black tile in Figure 1(b) represents a mountain, hence the robot can move only to the five white tiles indicated by the arrows. In contrast, the robot can move to seven tiles in Figure 1(c).

<img width="482" alt="rules-robot" src="https://user-images.githubusercontent.com/69590474/90357676-28f43d00-e097-11ea-86fb-30d9765231a6.png">

Path cost:

Robot’s wheels are built so that a diagonal move is the easiest. Hence, the cost of such a move is 1. Any other move has a cost of 2.

Input:

• The first line will contain one number that specifies the number of rows and columns in the map.
• Subsequent lines will contain the map, one line per row. The following values will be accepted for each tile:

![tile](https://user-images.githubusercontent.com/69590474/90357879-b768be80-e097-11ea-94f2-e99344fac421.jpg)


