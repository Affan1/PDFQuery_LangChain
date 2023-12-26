# UK Budget File Analysis with OpenAI, LangChain, and CassandraDB

## Overview

This project demonstrates an innovative approach to processing and analyzing the UK Government's budget document, a PDF file, using OpenAI's API and LangChain. The extracted information is then vectorized and stored in CassandraDB for efficient querying and analysis.

## Key Features

- **PDF Parsing**: Utilizing OpenAI's advanced natural language processing capabilities to read and interpret the UK budget PDF.
- **LangChain Integration**: Leveraging LangChain for streamlined processing and chaining of language models.
- **Data Storage in CassandraDB**: Efficiently storing and retrieving vectorized data from the budget document.

## Getting Started

### Prerequisites

- Python 3.10 or later
- Access to OpenAI's API
- CassandraDB installed and running
- LangChain library

### Installation

1. **Clone the Repository**

   ```sh
   git clone https://github.com/Affan1/UK-Budget-File-Analysis-with-OpenAI-LangChain-and-CassandraDB.git
   cd uk-budget-analysis
   ```

2. **Install Required Python Libraries**

   ```sh
   pip install -r requirements.txt
   ```

3. **Environment Setup**
   - Create a `.env` file in the project root.
   - Add your OpenAI API key and CassandraDB credentials:
     ```
     OPENAI_API_KEY=your_api_key_here
     CASSANDRA_HOST=your_cassandra_db_host
     CASSANDRA_PORT=your_cassandra_db_port
     ```

### Usage

1. **Reading the UK Budget PDF**

   - Place the UK budget PDF file in the project directory.
   - Run the script to process the PDF:
     ```python
     python read_budget.py
     ```

2. **Data Processing with LangChain**

   - The script uses LangChain for chaining language models to process and understand the content.

3. **Storing Data in CassandraDB**
   - Extracted data is vectorized and stored in CassandraDB for future analysis.

## CassandraDB Schema

- The CassandraDB schema is designed to optimize for querying vectorized data from the budget document.
- Example schema:
  ```astra_vector_store = Cassandra(
    embedding=embedding,
    table_name="qa_mini_demo",
    session=None,
    keyspace=None,
  );
  ```

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Muhammad Affan Raza - [@Linkedin](https://www.linkedin.com/in/muhammad-affan-raza/)

Project Link: [https://github.com/Affan1/UK-Budget-File-Analysis-with-OpenAI-LangChain-and-CassandraDB](https://github.com/Affan1/UK-Budget-File-Analysis-with-OpenAI-LangChain-and-CassandraDB)
