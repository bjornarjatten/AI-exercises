# Mandatory Assignment 1

**Name:** Bjørnar Haugstad Jåtten \
**ITU-username:** bjja@itu.dk

------------------

A. **Weighted A\* corresponds to**:

- When w = 1, weighted A\* corresponds to greedy best-first search: h(n)

- When w = 0.5, weighted A\* corresponds to normal A\* search: g(n) + h(n)

B. We know that we use an admissible heuristic, thus we know that A\* search is the optimal algorithm, meaning that the algorithm always find a least-cost solution. To get a A\* search, we have to give the weighted A\* algorithm w = 0,5. This means that 0.5 is the value in which the weighted A\* is optimal.