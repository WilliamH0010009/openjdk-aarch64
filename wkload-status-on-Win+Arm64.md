|Workload| Tests |  Arm64 | Comments  | 
|:--:|:--:|:--:|:--:|
| SPECJBB2015 |  |o*  | Performance difference observed on a [TX2](https://github.com/microsoft/openjdk-aarch64/blob/master/Arm64_systems.md) running Linux | 
| SPECJBB2005 |  | o* | Performance difference observed on a TX2 running Linux |  
| SPECJVM2008 | crypto, xml, derby, compress, etc | o* | startup doesn't work on JDK8+ (we are at JDK16/current tip) | 
| SPEC SERT | CPU/LU/SORT/SSJ/Flood3/Capacity/compress/Sha256 |o* |Benchmark changes made to accomodate the new platform combo, upstream to SPEC, benchmark needs fixing with removal of Nashorn| 
| DaCapo Benchmark | avrora fop h2 jython luindex lusearch lusearch-fix pmd sunflow tomcat xalan  | o* | one benchmark utilizes an x86-64 dll. A few others don't work on JDK8+. Lower priority |
| Scimark2 |  |o  |  | 
|Java MicroBenchmark Harness (JMH) | many microbenchmarks used for performance and implementation testing | o* | we ran the 'jmh-jdk-microbenchmarks' suite on our [test platforms](https://github.com/microsoft/openjdk-aarch64/blob/master/Arm64_systems.md) and found no significant issues |
|Java Regression Testing Framework (JTREG)| | o*| part of our CI|
|JFC applications and applets ([demo/jfc](https://docs.oracle.com/javase/7/docs/technotes/samples/demos.html))| | o | VEH and SEH bug identified and fixed |
|The Computer Benchmarks Game|10 Java sub-benchmarks| x|Enablement and characterization work|
|[Renaissance Suite](https://renaissance.dev/)|| x|Enablement work has started |
|VSCode| | o | |
|Minecraft Server| | o | |

_Key to Status:_
|Legend| Status |
|--|--|
| o | Complete |
| o* | Almost there, see notes |
| x | Incomplete | 
