# Model-Collapse

Welcome to model collapse, an experimental project to create a prompt based network with distillation over every node.

We want the resulting model to both be far smaller than existing models, and far more interpratable.

The search space of a regular model makes it very hard to understand. Instead of searching through millions of weights and biases, I want to simply have the model explain itself.

TODO:

- [ ] migrate current "inference" to mistral (or another open source model)
- [ ] optimize gating mechanism distribution by running inference over a common dataset, and getting equal results for every category
- [ ] optimize logic over generated chain of thought responses by testing in the Eleuther Harness
- [ ] route an open source dataset (likely amberChat dataset) and seperate into datasets over a parent model (whoever is highest on the opensource hf leaderboard)
- [ ] train each node using the mamba architecture (because these responses will likely be loooong)
- [ ] repeat this process over each node with the subset of training data routed to it, to further simplify the network