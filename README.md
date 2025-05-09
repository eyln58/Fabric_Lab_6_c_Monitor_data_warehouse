# 🧩 Exploring Dynamic Management Views and Query Insights in Microsoft Fabric

This repository documents the completion of a hands-on lab focused on monitoring and observing **query activity, connections, and performance** in a Microsoft Fabric data warehouse using **Dynamic Management Views (DMVs)** and **Query Insights**.

## 🎯 Purpose of the Lab

The main goal of this lab was to understand how Microsoft Fabric enables **monitoring, diagnostics, and performance analysis** at the SQL level. Through a series of explorations using DMVs and built-in views, this exercise demonstrated how to track active connections, sessions, and long-running or frequently executed queries.

## 🧠 What I Learned

During this lab, I gained practical exposure to:

- **Creating and Exploring a Sample Data Warehouse**  
  Started by creating a Fabric data warehouse pre-populated with a taxi ride dataset for testing and observation.

- **Using DMVs (Dynamic Management Views)**  
  Queried key DMVs such as:
  - `sys.dm_exec_connections`
  - `sys.dm_exec_sessions`
  - `sys.dm_exec_requests`  
  to monitor real-time activity and understand how connections, sessions, and query execution are tracked internally.

- **Joining DMVs for Deeper Analysis**  
  Combined multiple DMVs to generate a consolidated view of currently running queries, identifying execution time, users, and sessions.

- **Simulating Load with Long-Running Queries**  
  Ran an intentionally infinite query to simulate workload, and observed how its runtime grew over time in DMV outputs — then canceled and confirmed the session ended correctly.

- **Exploring Query Insights Views**  
  Discovered and queried built-in views under the `queryinsights` schema, including:
  - `exec_requests_history`: Previously executed queries
  - `frequently_run_queries`: Most common query patterns
  - `long_running_queries`: Performance bottlenecks and inefficiencies

## ✅ Outcome

By the end of the lab, I gained a solid understanding of:
- How Microsoft Fabric surfaces low-level SQL activity in a cloud-native warehouse
- How to use DMVs to track live queries, diagnose issues, and monitor usage
- How to leverage historical insights for identifying optimization opportunities

This knowledge is critical for **performance tuning, resource monitoring, and operational transparency** in production analytics environments.

## 🤝 Let’s Connect

If you’re interested in Microsoft Fabric, performance monitoring, or data engineering at scale, feel free to reach out and connect.  
Let’s talk Fabric and observability on [LinkedIn](https://www.linkedin.com/in/eyilan/).
