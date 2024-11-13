
graph LR
    A[المستخدم] --> B[Ingress LSR (إضافة التسمية)]
    B --> C[LSR 1]
    C --> D[LSR 2]
    D --> E[Egress LSR (إزالة التسمية)]
    E --> F[المستقبل]

    subgraph MPLS Path
        B
        C
        D
    end

    classDef mplsPath fill:#f9f,stroke:#333,stroke-width:2px;
    class B,C,D mplsPath;

