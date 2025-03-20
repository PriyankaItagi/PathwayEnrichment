# Pathway Enrichment Analysis Shiny App

This is an R Shiny app designed for performing pathway enrichment analysis using gene ontology (GO) terms. It allows users to upload a list of genes, select an organism and ontology, and visualize enriched pathways using interactive plots and tables.

## Features
- **Gene List Input**: Paste or upload a list of gene IDs in Entrez format.
- **Organism Selection**: Choose between human (`org.Hs.eg.db`) and mouse (`org.Mm.eg.db`) databases.
- **Ontology Selection**: Perform enrichment analysis for Biological Process (BP), Molecular Function (MF), or Cellular Component (CC).
- **Enrichment Plot**: Visualize enriched pathways using a dot plot.
- **Enrichment Table**: View detailed enrichment results in an interactive table.
- **Error Handling**: Provides user feedback for invalid inputs or errors.

## How to Use
1. **Paste Gene List**:
   - Enter a list of gene IDs (one per line) in the input box. Example:
     ```
     7157
     7422
     3320
     29110
     ```

2. **Select Organism and Ontology**:
   - Choose the organism database (Human or Mouse).
   - Select the ontology (Biological Process, Molecular Function, or Cellular Component).

3. **Run Analysis**:
   - Click the **Run Enrichment Analysis** button to perform the analysis.

4. **View Outputs**:
   - **Enrichment Plot**: A dot plot showing the top 20 enriched pathways.
   - **Enrichment Table**: A table with detailed results, including p-values, adjusted p-values, and gene counts.

## How to Run the App
1. Clone this repository to your local machine -
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
2. Open the app.R file in RStudio or your preferred R environment.

3. Install the required R packages if you don't already have them -
```R
install.packages("shiny")
install.packages("clusterProfiler")
install.packages("org.Hs.eg.db")
install.packages("ggplot2")
install.packages("DT")
install.packages("shinythemes")
```
4. Run the app -
In RStudio, click the Run App button.
Alternatively, run the following command in the R console:
```R
shiny::runApp("path/to/your/app.R")
