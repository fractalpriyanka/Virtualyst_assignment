flowchart TD
A[Start] --> B[Load MNIST CSV Dataset]

    B --> C[Data Exploration]
    C --> D[Data Preprocessing]

    D --> D1[Normalize Pixel Values]
    D --> D2[Train-Test Split]

    D --> E[PCA (Optional)]

    D --> F[Baseline Model Training]
    E --> G[PCA-Based Model Training]

    F --> H[Model Evaluation]
    G --> H

    H --> I[Performance Comparison]
    I --> J[Error Analysis]

    J --> K[Final Report]
    K --> L[End]
