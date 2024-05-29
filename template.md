### Mermaid Vs Code

```mermaid
flowchart LR
%% Colors %%
classDef blue fill:#2374f7,stroke:#000,stroke-width:2px,color:#fff
classDef orange fill:#fc822b,stroke:#000,stroke-width:2px,color:#fff

%% Project database %%
G[(Goals)]:::blue --> |Connects to| P(projects):::orange

P --> |Has| PT(Tasks)
PT ---- |Is| IC([Incomplete]) & C([Complete])
C ---> |Needs| R[[Review]]

R -.-> |Creats| G