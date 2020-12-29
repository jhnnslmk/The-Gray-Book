# Nodes

Nodes are the main building blocks of a patch. There are different types of nodes:

*Image:Static Operation node, process node, record node, class node*

## Operation Nodes
Operation nodes are nodes representing a single operation.

It is useful to distinguish static operation nodes from all other operation nodes. They have a lighter look that indicates that they are not operating on a state, ie. they do not store any data between consecutive calls.

Record and class nodes are part of a record or class respectively, on which they operate. The name of the datatype is what is written in smaller letters below the nodes name.

## Process Nodes
A process node represents a single instance of a patch. The name _Process_ comes from the fact that it can be understood like a little machine that continues to run (update) after it was created and saves its state from one frame to the next.

See also [Datatype Patch](patches.md).

---

Any node that spots an arrow icon has a patch behind it which can be reached by a simple middle-click or via the context-menu: Open.

*Image:Node with a patch behind it*

## Pin group
To set a pin of type Spread up as a pingroup you can add and remove pins to using <span class="keyseq"><kbd>CTRL</kbd><kbd>+</kbd></span> or <span class="keyseq"><kbd>CTRL</kbd><kbd>-</kbd></span> respectively (like Group or Cons nodes), simply inspect the pin using the Configure Menu and set the flag "Pin Group" to TRUE.

## Apply pin
Nodes whose first input and first output share the same datatype can have an _Apply_ pin added via the `context-menu > Configure`. If apply is set to false, the operation is bypassed and the input returned unchanged as the output.
