# Levels of Testing : 

# 1. Unit Testing : (white box technique)
   - a unit is single module or component of software
   - unit testing is conduted on single program or single module
   - it is white box testing technique conducted by developer
     
# Unit testing technique : 

1. Basis Path testing
2. control structure testing
3. conditional coverage
4. loops coverage
5. mutation

# 2. Integration Testing : 
- Integration testing is performed between 2 or more module
- It focuses on checking data communication between multiple module
- It is white box testing technique
- Main Purpose of Integration Testing :
To check moudules are communicating each other as DFD Data Flow Diagram which is specified in
TDD ( Technical Document Diagram )

 # Types of Incremental Testing
 - Inceremental Inegration testing
 - Non Inceremental Integration testing

# When to Perform Incremental Testing

- Software incremental testing involves interlinking each component individually rather than combining them all at once.
- This is performed only if all the defects detected at the unit testing phase have been fixed.
- The best time to use incremental testing is when software components are still being developed.
- The drivers and stubs can be used for any unfinished components if required during testing.
- For example, if modules 2 and 3 are still under development during the testing phase of modules 1, 2, and 3.
- In that case, drivers can be combined with module 1 to replicate the unfinished module and continue the integration process.

 # 1. Inceremental Inegration testing
 - Incrementally adding the module and testing the data between the module
 - It has 2 approches :
 - TOP - DOWN
 - BOTTOM UP

   # TOP DOWN Inceremental Inegration testing :
   
   - Top-Down Incremental Integration Testing means you start testing from the top-level modules and add lower-level modules step by step. You use stubs to simulate modules that aren’t ready yet. As you move down, you replace stubs with real modules and keep testing.
   - Stubs are used as a substitute if any lower-level module is unavailable for testing or under development.
   - Stubs, also called programs, are dummy programs that replace any lower-level module in a top-down hierarchy.
   - They are as higher-level modules call them to check the interface and integration.
   - For example,
  - If you have already checked the Log module and need to integrate it with the FPP module, but FPP is still under development,
  -  a stub can be used to replace FPP. In this case, the integration hierarchy will go down with Log, PLP, and PDP modules.
  -  If any other lower-level modules are missing, they can also be replaced by stubs.

<img width="689" height="797" alt="image" src="https://github.com/user-attachments/assets/2aec3636-1f2f-4fce-87c4-b71630670f11" />


# BOTTOM UP Inceremental Inegration testing :
- The bottom-up method of Incremental Testing moves in an upward manner.
- In this method, the lower-level modules are tested first and integrated with higher-level modules.
- This is the right approach when bottom-level subsystems are test-ready.
- In this case, stubs are not required because the lower-level modules are already running.
- However, if higher-level subsystems are not ready for testing and integration, drivers (called calling programs) replace them.
- For example,
- In the bottom-up approach, the testing will begin with the Pay and Cart modules.
- Once tested, they are integrated with the PDP module.
- After this, PDP is tested with PLP, and the process is repeated until all modules are integrated, ending with the Log module—the highest-level subsystem in the application.
  
  <img width="644" height="763" alt="image" src="https://github.com/user-attachments/assets/899793d5-a20b-4b99-a80a-86f593eff1b8" />


# 3. Sandwich Testing

- Sandwich testing methodology combines top-down and bottom-up testing approaches.
- It is also known as hybrid integration testing.
- In sandwich testing, there are three distinct layers involved:
- Main target layer – the core layer being tested.
- Layer above the target – the higher-level interface or module.
- Layer below the target – the lower-level functions or modules.
  
-  The process starts by testing the user interface (top layer) using stubs, which simulate the middle and lower layers.
-  Next, the lowest-level functions (bottom layer) are tested using drivers, which mimic the upper layers.
-  Finally, once all layers are integrated, the main target (middle layer) is tested as part of the whole system, ensuring proper interaction between all layers.
