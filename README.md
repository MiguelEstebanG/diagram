Example of mermaid diagram

```mermaid

graph TD;

    class jojo fill:#ff, stroke:#fff, stroke-width:0.5px, font-size: 20px;


    A-->B;
    A-->C;
    B-->D;
    C-->D;

    subgraph T[hola]
        A(funcionas?)
        subgraph G[ ]
            B(creo que sí)
        end
    end

    linkStyle default stroke-width: 1px;

```
