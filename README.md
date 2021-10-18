# uniform-cost-search-algorithm
Evolves in amplitude algorithms. The uniform cost search algorithm expands each time the node n with the lowest current path consumption g (n).
Data structure:
border: border, storing unexpanded nodes. By maintaining a priority queue, it is organized according to route loss.
explored: explore set, save the visited node.
Flow algorithm:
If the border is empty, it returns the fault. Operation: EMPTY? (Border)
Otherwise, select a leaf node from the edge. Operation: POP (border)
Target test: pass again, otherwise put leaf node state in scan set
Traverses all actions of the leaf node
    Each action produces child nodes

If the state of the child node is not in the scan set or on the edge, it is inserted into the edge set. Operation: INSERT (child, border)

If the state exists in the edge set and there is higher path consumption, the child node overrides the state in the edge set
