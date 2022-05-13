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
      * SQL ( For faster reads and ready heavy systems)  vs No SQL  ( Faster Writes and Write heavy system )
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

