# Microsoft-Azure-Data-Fundamentals
1. Explore core data concepts
    - Explore file storage : Delimited text files, JSON,XML, BLOB
    - Common data format
    - Store data in database : relation, no-sql
    - Explore analytical data processing : Datalake -> データ処理（ELT、ETL） -> analyst (by load data form dataware house)
        + ETL transforms data on a separate processing server, while ELT transforms data within the data warehouse itself.(ETL は別の処理サーバーでデータを変換しますが、ELT はデータ ウェアハウス自体の中でデータを変換します。)
        + ETL does not transfer raw data into the data warehouse, while ELT sends raw data directly to the data warehouse.(ETL は生データをデータ ウェアハウスに転送しませんが、ELT は生データをデータ ウェアハウスに直接送信します。)
2. Explore job roles in data
    - Database administrators manage databases, bakcup, restore.
    - Data engineers: pipelinr, clean data, make rule
    - Data analysts : crate visulization, chart to make true decesions.
3. Data service
    - Azure Cosmos DB : no-sql
    - Azure Data Factory: to build extract, transform, and load (ETL) 
    - Azure Synapse Analytics : make pipeline, sql, spark..
    - Azure Databricks :  create analytical data
    - Azure HDInsight : hadoop. large data
    - Microsoft Power BI : visualizations
4. Relational data in azure
5. Non-relational data in azure
6. Explore data analyst in azure
    - warehousing architecture : ELT
    - data ingestion pipelines 
        -  Azure Blob Store linked service to ingest the input dataset, 
        -  Azure SQL Database: データ分析
        - Azure Databricks(is analyst tool, Azure Databricks cleans and transforms structureless data sets) or Azure HDInsight, or apply custom logic using an Azure Function. 
        - Output data to datawarehouse, such as Azure Synapse Analytics. 
7. Data stores
    - Data warehouses : A data warehouse is a relational database in which the data is stored in a schema that is optimized for data analytics rather than transactional workloads.(データ ウェアハウスは、トランザクション ワークロードではなくデータ分析用に最適化されたスキーマにデータが格納されるリレーショナル データベースです。)
    - Data lakes: A data lake is a file store, usually on a distributed file system for high performance data access. Technologies like Spark or Hadoop are often used to process queries on the stored files and return data for reporting and analytics (データ レイクはファイル ストアであり、通常は高性能データ アクセス用の分散ファイル システム上にあります。 Spark や Hadoop などのテクノロジは、保存されたファイルに対するクエリを処理し、レポートや分析用のデータを返すためによく使用されます。)
    
8. Azure services for analytical stores
    - Azure Sysnapse Analystic: datawarehouse
    - Azure Databricks: Datalake ( analyst spark, hadoop)
    - Azure HDInsight: it can be a suitable option if your analytics solution relies on multiple open-source frameworks or if you need to migrate an existing on-premises Hadoop-based solution to the cloud.(分析ソリューションが複数のオープンソース フレームワークに依存している場合、または既存のオンプレミスの Hadoop ベースのソリューションをクラウドに移行する必要がある場合に適したオプションです。)
9. Explore fundamentals of real-time analytics
    - Batch processing, in which multiple data records are collected and stored before being processed together in a single operation. (複数のデータ レコードが収集され、1 回の操作でまとめて処理して、保存されます。)
            - best for large write
            - high latency(高レイテンシ)
    - Stream processing, in which a source of data is constantly monitored and processed in real time as new data events occur.(新しいデータ イベントが発生すると、データ ソースが常に監視され、リアルタイムで処理されます。)
            - 遅延が遅い
            - Real time.
            - tool: Azure Stream Analytics, Azure IoT Hub, Azure Event Hubs, Apache Kafka:
10. Explore fundamentals of data visualization
    - Microsoft Power BI :データ視覚化(しかくか)を構築するために使用できるツールです。
    - Analytical modeling in Microsoft Power BI
        - Tables and text
        - Bar and column charts
        - Line charts
        - Pie charts
        - Scatter plots.
        - Maps
    - Interactive reports in Power BI
        - ![image](https://user-images.githubusercontent.com/44230257/197465819-1f8b912f-1305-41dc-9762-8a409d75d0f0.png)

11. BI Practice
    - Data: 
        - https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals/raw/master/power-bi/customers.csv
        - https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals/raw/master/power-bi/products.csv
        - https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals/raw/master/power-bi/orders.csv
    - Importすると
    - ![image](https://user-images.githubusercontent.com/44230257/197466146-16ac4831-d39c-4767-813f-c555bdb98732.png)
    - ![image](https://user-images.githubusercontent.com/44230257/197466196-302281b7-2031-4e64-8110-b1f2839dc0c0.png)
    - Visualization（視覚化）しかくか
    - ![image](https://user-images.githubusercontent.com/44230257/197466321-698c8f66-4cce-4936-a39b-3e78b63e4ea0.png)
