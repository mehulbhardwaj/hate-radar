# Interactive Data Visualization: Indophobic Discourse in Western Digital Spaces (2015-2025)

## Project Overview

This repository hosts a self-contained, single-file web application that visualizes the **Exploratory Thematic Index (ETI)**. The ETI is an _ad hoc_ metric used for risk assessment and trend identification regarding anti-Indian sentiment in Western digital media.

The primary goal of this repository is to serve as a **proof-of-concept visualization framework** that must eventually be decoupled from its synthesized data and connected to a robust, quantifiable data source (ETI 2.0).

## 🚀 Getting Started

Since the project is implemented as a single, self-contained HTML file (using Tailwind CSS and Chart.js via CDNs), no build steps or dependencies are required.

### Viewing the Report

To view the full report, the interactive ETI chart, and the thematic deep dives:

1.  Clone this repository:
    
        git clone [your-repo-link]
        
    
2.  Navigate to the project directory.
    
3.  Open the main file in any modern web browser:
    
        open "./Indophobic Discourse in Western Digital Spaces: A Longitudinal Exploratory Analysis (2015-2025).html"
        
    

## 📂 Repository Contents

The repository contains a single file:

| Filepath | Description |
| --- | --- |
| Indophobic Discourse in Western Digital Spaces: A Longitudinal Exploratory Analysis (2015-2025).html | Contains all HTML structure, Tailwind CSS styling, and JavaScript logic (including data structures for the ETI chart and the accordion components). |

## ⚠️ Important Note on Data & Methodology

The data displayed in the ETI chart is **synthesized from secondary academic literature** and is hardcoded directly into the JavaScript within the HTML file. It is explicitly labeled as an **Exploratory Thematic Index (ETI)** and should not be treated as statistically validated or quantifiable primary evidence.

### Hardcoded Data Structure (Located in `...html` file)

The data currently resides in a JavaScript object structured as follows:

    const data = {
        years: [2015, 2016, 2017, ...],
        regions: [
            { name: 'US', values: [...] },
            // ... other regions
        ],
        analysis: {
            // Detailed hover-over text for each data point
        }
    };
    

## 🛠️ Contribution and Future Work

The current implementation is stable but relies on mock data. Contributions are highly encouraged to transition this project into a viable research tool.

### Primary Contribution Goals (ETI 2.0)

1.  **External Data Integration:** Replace the hardcoded `data` structure with a mechanism to fetch and parse external data (e.g., JSON or CSV) from a dedicated API or database (e.g., Firebase Firestore or a custom API endpoint).
    
2.  **Validated Data Pipeline:** Design and implement a service layer to handle the ingestion of quantifiable primary data (e.g., N-gram frequency counts, validated sentiment scores) to create a robust, statistically sound **ETI 2.0**.
    
3.  **Refactoring:** Separate the core JavaScript visualization logic from the presentation layer to improve maintainability.
    
4.  **Accessibility:** Review and improve the semantic structure and ARIA attributes for better accessibility, particularly around the interactive chart and collapsible sections.
    

### Contribution Guidelines

1.  Fork the repository.
    
2.  Create a feature branch (`git checkout -b feature/your-feature`).
    
3.  Commit your changes (`git commit -m 'feat: added external data fetching service'`).
    
4.  Push to the branch (`git push origin feature/your-feature`).
    
5.  Open a Pull Request.
    

## 📜 License

This project is licensed under the MIT License.
