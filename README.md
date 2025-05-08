# PROM subgraph example

This is an example subgraph for PROM network

## Configuration

- `subgraph.yaml`: The main configuration file for the subgraph. It defines the data sources, event handlers, and mappings.

For the PROM network, the subgraph should point to the `prom` network.

```yaml
# ...
dataSources:
  - kind: ethereum
    network: prom
# ...
```

## Getting Started

1. Install dependencies

```bash
yarn install
```

2. Build the subgraph

```bash
yarn codegen
```

3. Create subgraph

```bash
yarn subgraph:create --subgraph vprom  --access-token your-secret-token
```

3. Deploy the subgraph

```bash
 yarn deploy --headers '{"Authorization": "Bearer yous-secret-token"}'  --deploy-key your-secret-token
```

4. Access the subgraph

```bash
open https://node.graph.prom.io/subgraphs/name/vprom
```
