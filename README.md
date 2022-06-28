# SD-Template
Template that can be used to design a system


*  Identify Functional requirements
*  Identify Non functional & operational requirements    
      * Availability
      * Performance
      * Latency
      * Legal & Compliance & Privacy
      * Maintanence * data lifecycle)
      * Capacity
      * Security
      * Geo
      * Analytics and ML
*  Identify extended requirements
*  Calculate Capacity Estimates based on Reads / Writes
      * Calculate Traffic Estimates
      * Calculate Storage Estimates
      * Calculate Bandwidth Estimates
      * Calculate Memory Estimates
      * Find out the number of concurrent users ? Say X% of the DAU
      * Based on the concurrent users , calculate the QPS
*  Identify if the system is read or write heavy
*  Talk about the High Level Design
      * HLD components
      * API Design
      * DB models
          * SQL ( For faster reads and ready heavy systems)  vs No SQL  ( Faster Writes and Write heavy system ) 
          * Relational vs Document vs Graph
      * DB Design 
*  Basic Design Algorithm
*  Design Deep dive
     *  Uncover bottlenecks as the scale increases
            * API Servers Scaling - Stateless and Easy to scale based on CPu / IO and Load
            * Web socket servers scaling  - **Stateful** Easy to scale **however drain connections at LB ** before adding more nodes
     *  Sharding 
     *  Concurrency 
*  Latency
*  Cache
*  Load balancing
* Purging or DB cleanup
*  Monitoring and Alerting
*  Measure of success and design evolution

* Follow the design template below for a design document
     * Why are we doing this project ?
     * Stakeholders
     * Major Design Decisions
          * MVP Scope
     * Design
          * HLD
          * Flows and Sequences
          * APIs and Description
     * Release strategy
          * Development milestones
          * Sand box environments where people can explore and experiment safely
          * Testing
          * Deployment ( CI / CD ) 
     * Measurements of success
          * KPI to determine the success of the project
     * Monitoring / Observability
          * Requests per second
          * Cache hit rate
          * Error rate 
          * R/W in DB     
          * Head of line blocking ( A server can only process a small number of tasks in parallel limited by its CPU Cores often. It only takes a small no 
            of slow requets to hold up the processing of subsequent requests
          * Tail latencices ( high latencies that clients see fairly infrequently)  Ex: 1 in 1000 requests are slow . 
            Reducing response times at high percentiles is difficult because they are easily affected by random events outside our control and benefits are      
            diminishing
            
     * Open Questions
     * Other userful links
                          
    

