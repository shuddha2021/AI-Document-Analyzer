# AI Document Analyzer 📄✨

**AI Document Analyzer** is a comprehensive, interactive, and purely client-side web application designed for summarizing and analyzing text documents. Built entirely with HTML, CSS, and JavaScript, it leverages various frontend libraries to offer a rich set of features without requiring any backend processing, ensuring user data remains private and secure within the browser.

This tool serves as an impressive demonstration of what can be achieved with modern web technologies for NLP tasks, data parsing, and visualization, all within a single-file architecture.

<img width="955" alt="AI Document Analyzer Screenshot 1" src="https://via.placeholder.com/955x600.png?text=App+Screenshot+1+-+Input+and+Settings">
<!-- TODO: Replace with actual screenshots of your application -->
<img width="955" alt="AI Document Analyzer Screenshot 2" src="https://via.placeholder.com/955x600.png?text=App+Screenshot+2+-+Summary+and+Analysis">

## 🚀 Features

*   **Versatile Input Options:**
    *   Direct text pasting.
    *   Drag-and-drop or browse to upload files.
    *   Supports `.txt`, `.csv`, `.xlsx` (Excel), and `.html` files. (PDF support is planned with PDF.js integration).
*   **Advanced Summarization Techniques:**
    *   **Extractive Summarization:** Identifies and combines the most important sentences from the original text.
    *   **Simplified "Abstractive" Summarization:** A keyword-focused approach to generate concise summaries.
    *   **Bullet Point Summarization:** Extracts key information as easy-to-read bullet points.
    *   Adjustable summary length.
*   **In-Depth Text Analysis:**
    *   **Key Concept Extraction:** Identifies and displays the most relevant terms and concepts.
    *   **Named Entity Recognition (NER):** Basic regex-based extraction of common entities (Persons, Organizations, Dates, Locations, Misc).
    *   **Document Insights:**
        *   Readability Score (Flesch-like).
        *   Overall Sentiment Analysis (lexicon-based).
        *   Text Statistics (word count, sentence count, average words per sentence).
*   **Interactive User Interface:**
    *   **Responsive Design:** Adapts to different screen sizes.
    *   **Light/Dark Theme Toggle:** For user comfort.
    *   **Tabbed Layout:** Organizes input, settings, and various analysis results clearly.
    *   **Real-time Word Count:** As you type.
    *   **Loading Indicators & Progress Bars:** For a smooth user experience during processing.
*   **Data Visualization:**
    *   **Entity Distribution Chart:** Bar chart (via Chart.js) showing the frequency of different named entity types.
    *   (D3.js included for potential future advanced visualizations like word clouds or network graphs).
*   **Utility Features:**
    *   **In-Document Search:** Find specific terms within the original text with context.
    *   **Copy & Download:** Easily copy summaries or download them as `.txt` files.
    *   **Export All Results:** Download a comprehensive analysis report.
    *   **Processing History:** Saves recent analyses in `localStorage` for quick reloading.
*   **Client-Side Processing:**
    *   **Privacy-Focused:** All analysis happens directly in the user's browser. No data is sent to any server.
    *   **Offline Capable:** Once loaded, the application can function offline (for text input).

## 🛠️ Technologies Used

*   **Core:** HTML5, CSS3, JavaScript (ES6+)
*   **Machine Learning (Utility/Placeholder):** [TensorFlow.js](https://www.tensorflow.org/js) (included, not heavily used for complex model inference in this version)
*   **Charting:** [Chart.js](https://www.chartjs.org/) for entity distribution visualization.
*   **Advanced Visualization (Foundation):** [D3.js](https://d3js.org/) included for potential future graphical representations.
*   **CSV Parsing:** [PapaParse](https://www.papaparse.com/) for handling `.csv` files.
*   **Excel Parsing:** [SheetJS (js-xlsx)](https://sheetjs.com/) for reading `.xlsx` and `.xls` files.
*   **(Future) PDF Parsing:** Structure in place to integrate [PDF.js](https://mozilla.github.io/pdf.js/) if added via CDN.

## 💡 How It Works (Simplified AI)

The "AI" capabilities in this application are primarily implemented using:

1.  **Algorithmic NLP:**
    *   **Summarization:** Sentence scoring based on word frequencies (TextRank-like) and positional heuristics.
    *   **Key Concept Extraction:** Identifying high-frequency content words after stop-word removal.
2.  **Rule-Based Systems:**
    *   **Named Entity Recognition (NER):** Regular expressions are used to find common patterns for dates, emails, and rudimentary person/organization mentions.
3.  **Lexicon-Based Analysis:**
    *   **Sentiment Analysis:** Comparing words against predefined lists of positive and negative terms.
4.  **Statistical Methods:**
    *   **Readability & Text Stats:** Applying formulas (like a simplified Flesch score) and basic counting.

This approach allows for a feature-rich experience entirely within the browser, demonstrating fundamental NLP concepts without the overhead of large, pre-trained deep learning models.

## 🔧 Usage

1.  **No Installation Needed:** Simply open the `index.html` file in a modern web browser (Chrome, Firefox, Edge, Safari recommended).
2.  **Input Text:**
    *   Type or paste text directly into the "Text Input" area.
    *   Switch to the "File Upload" tab to drag-and-drop or browse for `.txt`, `.csv`, `.xlsx`, or `.html` files.
3.  **Configure Settings (Optional):**
    *   Adjust the desired **Summary Length** percentage.
    *   Set the maximum number of **Key Concepts** to extract.
    *   Choose the **Summary Type** (Extractive, Simplified "Abstractive", Bullet Points).
    *   Toggle options for **Extracting Named Entities** and **Calculating Document Insights**.
4.  **Analyze:**
    *   Click the "Analyze & Summarize" button.
5.  **View Results:**
    *   Navigate through the output tabs (Summary, Key Entities, Insights, Search Document) to explore the analysis.
    *   Interact with the entity chart.
    *   Use the search bar to find terms in your original document.
6.  **Manage & Export:**
    *   Copy or download the generated summary.
    *   Export a full text report of all analysis results.
    *   Access recently processed documents from the History section.

## 🖼️ Screenshots

<!-- Add more screenshots here -->
*Awaiting actual application screenshots. Placeholder images are currently used.*

<img width="955" alt="AI Document Analyzer Screenshot - File Upload" src="https://via.placeholder.com/955x400.png?text=File+Upload+Interface">
<br/>
<img width="955" alt="AI Document Analyzer Screenshot - Entity Chart" src="https://via.placeholder.com/955x400.png?text=Entity+Distribution+Chart">

## 🔮 Future Enhancements

*   **Integrate PDF.js:** Enable full text extraction from PDF documents.
*   **TensorFlow.js Model Integration:** Explore using lightweight pre-trained TF.js models for tasks like more advanced sentiment analysis or text classification.
*   **D3.js Visualizations:** Implement more dynamic visualizations like word clouds or interactive concept maps.
*   **Advanced NER:** Improve entity recognition accuracy and coverage, potentially with a small client-side model or more sophisticated rules.
*   **Topic Modeling:** Add functionality to discover underlying topics in the document.
*   **Improved Error Handling:** More granular error messages for file parsing and processing.
*   **UI/UX Refinements:** Continuous improvements to user experience and interface design.
*   **Web Worker Offloading:** Move computationally intensive tasks to Web Workers to prevent UI freezing on very large inputs.

## 🧑‍💻 About the Developer

This **AI Document Analyzer** was created by **Shuddha Chowdhury** ([@shuddha2021](https://github.com/shuddha2021)) as a demonstration of frontend development skills, NLP techniques, and building interactive, client-side AI-powered tools.

*   Portfolio: [shuddha2021.vercel.app](https://shuddha2021.vercel.app/)
*   GitHub: [github.com/shuddha2021](https://github.com/shuddha2021)

## 📜 License

This project is open-source and available for use/modification. Please refer to the licenses of the included third-party libraries (TensorFlow.js, Chart.js, D3.js, PapaParse, SheetJS) if you plan to redistribute or use them in your own projects.

The custom code for this project is provided under the [MIT License](LICENSE.md) (you would need to create a LICENSE.md file with the MIT license text).
