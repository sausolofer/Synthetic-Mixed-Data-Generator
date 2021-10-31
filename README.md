# Synthetic Mixed Data Generator

<p align="center"><img src ="SMDG_Img.png" width="70"/></p>

Synthetic Mixed Data Generator (SMDG) is an open-source tool distributed under [GNU General Public License](http://www.gnu.org/licenses/gpl.html) written in Java for producing supervised mixed datasets described by relevant, irrelevant, and redundant features.

## Requirements and Uses

### Prerequisites:
To clone, build, and compile the Project, the following software tools are needed:

* [Git](https://git-scm.com/downloads) 
* JDK 1.7 or above ([Oracle, ](https://www.oracle.com/java/technologies/downloads/#java8)[OpenJDK, ](https://adoptopenjdk.net/)[GraalVM](https://www.graalvm.org/java/quickstart/) or any other) 
* [Maven](http://maven.apache.org/download.cgi#Installation) (See this [tutorial](https://maven.apache.org/install.html) for installation)

Synthetic Mixed Data Generator requires:
* weka-stable 3.8.4
* commons-math3 3.2
* log4j 1.2.17
* opencsv 3.3
* flatlaf 0.37

### Source code:
Download the latest sources with the command:

`git clone https://github.com/sausolofer/Synthetic-Mixed-Data-Generator.git`

### Run and Uses:
* To use the Synthetic Mixed Data Generator in your Java code, see the file "Example.java" located in smdg.examples package.

* To Build and run the Maven Project from the Command Line, execute the following steps:

    1.- From the main directory of the project (i.e., where the pom.xml file is), compile the project and generate target folder using:
    
    `mvn compile`
   
    2.- Builds the maven project, cleans the target/ folder, and installs it into the local maven repository.  
    
    `mvn clean install`

    3.- In order to execute the Examples.java class, and in general, any main class generated in the target folder, the  Maven's exec plugin can be used as follows:
    
    `mvn exec:java -Dexec.mainClass=smdg.dataGenerators.Examples`
    
    Note 1: You must run the previous command from the main directory of the project, that is, where the pom.xml file is located.
    Note 2: If changes are made to the code, mvn compile needs to be executed again before calling exec.

    4.- To run the Graphical User Interface (SMDG-GUI), execute the SyntheticMDG.java file located in smdg.gui package with the following command.
    
    `mvn exec:java -Dexec.mainClass=smdg.gui.SyntheticMDG`


## Development

### Important links:
* Official source code repo: https://github.com/sausolofer/Synthetic-Mixed-Data-Generator
* Download releases: https://sourceforge.net/projects/smdg/files/latest/download



## Help and Support

### Documentation
* HTML documentation:

### Citation:
If you use the "Synthetic Mixed Data Generator" in a scientific publication, we would appreciate citations: 

    @article{solorio2022DataGenerator,
    title={A Multipurpose Synthetic Mixed Data Generator},
    author={Solorio-Fernández, Saúl and Carrasco-Ochoa, J. Ariel and Martínez-Trinidad, J. Francisco},
    year={2021},
    }

### Contact:
Feel free to reach out to ssolori1@asu.edu.com if you have any problems running the code or if you have a question about the repository as a whole. Lastly, if you have any suggestions to improve this repository, create an issue or send an email if that's more applicable.


