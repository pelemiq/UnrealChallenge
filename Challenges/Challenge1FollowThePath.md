# Challenge 1: Follow the path

To start with this Challenge, open the map located at Challenges/Challenge1/Challenge1.umap

On this challenge we have a classic videogame map with some specific points on it that we can visit

Looking inside the implementation, each navigation point is an actor, and has an array of references to other navigation points, that represents its connections


## Problem 1: Can I get there?

For this problem, you can navigate to BP_MapNode and reach to the isReachable function, you will realize that this function is not implemented yet, it looks that a lazy programmer created the placeholder function, it receives the other navigation point that we want to know if is connected to this one, but always return true.

Your mission is to get it working, on this map, if you play the level, you have you mouse available to click on any Navigation point, and you Character will move to the clicked point in case that the point is Reachable

To check if your solution is working, simply play the game, and click on the left side navigation points, the character should not move, as those points are not connected to the starting one.

<details>
  <summary>How do I know if two points are directly connected?</summary>
  
  For these example, we are using a [directed graph](https://en.wikipedia.org/wiki/Directed_graph) , meaning that  from a specific node, we can only go to the nodes on its Connections list.

  So, From A node, we can only directly go to B node if B is present inside A´s Connection list.
  
</details>


## Problem 1: Calculating the path



### Credits:
[Azgaar´s fantasy map generator](https://azgaar.github.io/Fantasy-Map-Generator/)