-> Set up the properties of the project to produce simpler to understand assembly??????

-> NOTE TO SELF: Revert these settings later to get the hang of understanding real assembly


#### Disable [[ASLR|ASLR]]
##### (NEVER do this in Production Builds)
1. Right Click project in Solution Explorer and go to properties (Alt + Enter)
2. Linker -> Advanced
3. Set "Randomized Base Address" to "No (/DYNAMICBASE:NO)"


#### Disable Just My Code Debugging
1. Go to the Solution/Project Properties
2. C/C++ -> General
3. Set "Support Just My Code Debugging" to "No"


#### Disable Security Check (IDK WTF THIS MEANS)
##### NEVER DO IT IN PRODUCTION
1. Properties -> C/C++ -> Code Generation
2. Set "Basic Runtime Checks" to "Default"
3. Set "Security Check" to "Disable Security Chec (/GS-)"


#### Disable Incremental Linking (IDK WTF THIS MEANS)
1. Properties -> Linker -> General
2. Set "Enable Incremental Linking" to "No (/INCREMENTAL:NO)"