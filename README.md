Correlation between metrics of Various Projects
=======================
The aim of this project is to measure different projects using different metrics and to co-relate them.
Here we perform various different coverage tests for developing test cases so that entire code is covered and there are no parts of the code left uncovered. The coverage helps us to make better test suites that can detect the anomalies and code mutants injected in the main code. The various coverages used to for code coverage are: 
1. **Statement Coverage:** measurement procedure wherein the number of lines of code covered under certain circumstances is calculated based on the inputs from the users.
2. **Branch Coverage:** Branch coverage is a measurement to calculate the number of branches executed per user input.
3. **Mutation Score:** Mutation score is a testing practice wherein we check the accuracy or precision of the test cases.
4. **Cyclomatic Complexity:** Cyclomatic Complexity is the measure number of linearly independent paths that can be executed in a program.
5. **Metrics based Software Maintenance Effort Model** 
6. **Software Defect Density**

#### Various Projects Used:
1. **Apache Commons Logging** - [*project details*](https://commons.apache.org/proper/commons-logging/) , [*source-code*](https://github.com/apache/commons-logging) 
2. **Apache Commons Lang** - [*project details*](https://commons.apache.org/proper/commons-lang/) , [*source-code*](https://github.com/apache/commons-lang)
3. **Apache Commons Collections** - [*project details*](https://commons.apache.org/proper/commons-collections/) , [*source-code*](https://github.com/apache/commons-collections)
4. **Apache Commons Math** - [*project details*](http://commons.apache.org/proper/commons-math/) , [*source-code*](https://github.com/apache/commons-math)
5. **JFreeChart** - [*project details*](http://www.jfree.org/jfreechart/) , [*source-code*](https://github.com/jfree/jfreechart)

#### Directory layout
    .
    ├── Data                               # Metrics of various project (alternatively `dist`)
    ├── DataAnalysisNoteBook               # jupyter notebook source Code     
    ├── Project Source Code for Analysis   # latest version of project
    ├── Docs                               # Documentation files (alternatively `doc`)
    └── README.md
    
#### Prerequisites and Installation Steps for EclEmma (JaCoCo)
1. Prerequisites : EclEmma requires Eclipse 3.8 or higher and Java 1.5 or higher. It has no dependencies on a particular operating system. Of course your Eclipse installation needs to contain the Java development tools (JDT) which is included in the default SDK installation.
2. Installation Steps: 
```
    Step 1. From your Eclipse menu select Help → Eclipse Marketplace.
    Step 2. Search for "EclEmma".
    Step 3. Hit Install for the entry "EclEmma Java Code Coverage".
    Step 4. Follow the steps in the installation wizard.
```
3. Verification : The installation was successful if you can see the coverage launcher in the toolbar of the Java perspective.

#### Configuration for PIT Testing
1. PIT requires Java 5 or above and either JUnit or TestNG to be on the classpath.
2. Add the plugin to build/plugins in your pom.xml
```
<plugin>
    <groupId>org.pitest</groupId>
    <artifactId>pitest-maven</artifactId>
    <version>LATEST</version>
 </plugin>
 ```
 3.  Mutation Coverage : It can be run directly from the commandline
 ```
 mvn org.pitest:pitest-maven:mutationCoverage
```

#### Installation and Configuration for CLOC
1. Depending your operating system, one of these installation methods may work for you:
```
  npm install -g cloc                    # https://www.npmjs.com/package/cloc
  sudo apt-get install cloc              # Debian, Ubuntu
  sudo yum install cloc                  # Red Hat, Fedora
  sudo pacman -S cloc                    # Arch
  sudo pkg install cloc                  # FreeBSD
  sudo port install cloc                 # Mac OS X with MacPorts
```  
2. To run cloc on Windows computers, one must first open up a command (aka DOS) window and invoke cloc.exe from the command line there.
```
prompt> cloc
Usage: cloc [options] <file(s)/dir(s)> | <set 1> <set 2> | <report files>
Input Options :
               --diff <set1> <set2>
               --csv  :  Write the results as comma separated values.
               --out=<file>  :  Synonym for --report-file=<file>.
```
#### Team Member Details
```
1. Chetan Paliwal : chetanpaliwal22@gmail.com
2. Himen Hitesh Sidhpura : himens72@gmail.com
3. Sandeep Siddaramaiah : sandeepsiddaramaiah@gmail.com
4. Karthik BP : karthikbeepi@gmail.com
5. Rohan Paspallu : paspallu.rohan@gmail.com
```


