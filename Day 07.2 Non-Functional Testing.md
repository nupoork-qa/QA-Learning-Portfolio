# Non - Functional Testing
- once the application funcationality is stable then we do non - functional testing.
- Focus on performance , load it can take and security etc .

 # Types of Non -  Functional Testing
 
 
1. Performance Testing  
   • Load Testing  
   • Stress Testing  
   • Endurance Testing  
   • Spike Testing  
   • Volume Testing  

2. Security Testing  

3. Recovery Testing  

4. Compatibility Testing  

5. Configuration Testing  

6. Installation Testing  

7. Sanitation/Garbage Testing  

  # Types of Software Testing

## 1. Performance Testing

### Load Testing
Load testing is a type of performance testing which involves evaluating the performance of
the system under the expected workload.  
A typical load test includes determining the response time, throughput, error rate, etc during
the course of the load test.

**Example:** For a newly developed application with an anticipated load of around 1000
concurrent users, we will create a load test script and configure it with 1000 virtual users and
run it for a 1-hour duration. After the test completion, we can analyse the result to determine
how the application behaves at the expected peak load.

---

### Stress Testing
Stress testing evaluates the application’s performance at a load much higher than the expected load.  
It also determines the **break-point** of the application — the point at which it fails to respond correctly.

**Example:** For an application with an anticipated load of 1000 users, we run the test with
1200 users and check if the application is robust enough to not crash.

---

### Endurance (Soak) Testing
Endurance testing determines if the system can sustain the continuous expected load for a long duration.  
It often reveals issues like **memory leaks**.

**Example:** For an application like income tax filing (used continuously for long durations),
we can run the test for 24–48 hours and monitor memory utilization.

---

### Spike Testing
Spike testing analyses the behaviour of the system when the number of users suddenly increases.  
It also checks if the application can recover after the sudden burst.

**Example:** For an e-commerce app running an ad campaign, the number of users may
increase suddenly. Spike testing helps validate such scenarios.

---

### Volume Testing
Volume testing is performed by feeding the application with a high volume of data.  
This helps identify bottlenecks when handling large data sets.

**Example:** For a new e-commerce application, we can insert millions of rows into the database
and then execute performance tests.

---

### Performance Testing Types - Summary

| Test Type        | Goal                        | Method                                | Load Level                |
|------------------|-----------------------------|---------------------------------------|---------------------------|
| Load Testing     | Understand performance under expected load | Gradual load increase | Expected Load |
| Stress Testing   | Identify breaking points    | Extreme/unrealistic load               | Beyond Expected Load |
| Endurance Testing| Assess long-term stability  | Sustained load over time               | Expected Load (long time) |
| Spike Testing    | Evaluate sudden traffic bursts | Short-duration spikes               | Sudden change in Load |
| Volume Testing   | Handle large data volumes   | Large datasets / transfers             | High data volumes |

---

## 2. Security Testing
- Checks if the software is secure and protects sensitive information.  
- Aims to find and fix vulnerabilities that could be exploited by hackers.  

**Focus Areas:**
- User Authentication  
- User Authorization / Access Control  
- Data Encryption & Decryption  
- Network Security  
- System Software Security  
- Client-side Security  
- Server-side Security  

**Example:** Testing an online banking app to ensure account data is protected from unauthorized access.

---

## 3. Recovery Testing
Assesses how well a system can recover after a failure or crash.  

**Failure Scenarios:**
- Power outage  
- Server unreachable  
- Network signal loss  
- Database server down  
- API failure  

**Example:** Simulating a sudden power outage and checking if a word processing app recovers the open document after restart.

---

## 4. Compatibility Testing
Ensures the software works across devices, browsers, and operating systems.  

**Focus Areas:**
- OS Compatibility  
- Browser Compatibility (Cross-browser)  
- Hardware Compatibility (Configuration Testing)  
- Backward Compatibility  
- Forward Compatibility  

**Example:** Testing a mobile app on multiple devices with different screen sizes.

---

## 5. Configuration Testing
Checks if the software works with different configurations and settings.  

**Example:** Testing a video game on different hardware setups to ensure smooth gameplay.

---

## 6. Installation Testing
Assesses the process of installing and uninstalling software.  

**Example:** Installing a new version of an app and checking if it installs without errors or conflicts.

---

## 7. Sanitation / Garbage Testing
Ensures that the software cleans up unused or leftover data.  

**Example:** Testing a messaging app to verify deleted messages are completely removed from the system.
