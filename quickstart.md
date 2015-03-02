---
title:
layout: default
---


Use From Maven Central 
=========================================

You must have Maven installed. ([See details here](http://nd4j.org/getstarted.html).)

Include an ND4J backend here:

     <dependency>
       <groupId>org.nd4j</groupId>
       <artifactId>nd4j-$BACKEND_OF_YOUR_CHOICE</artifactId>
       <version>${nd4j.version}</version>
     </dependency>

The possible backends right now are:

    nd4j-jcublas-${YOUR_CUDA_VERSION} 
    //(Ensure cuda is properly setup in your LD_LIBRARY_PATH)
    nd4j-jblas 
    //(Linux: Install Blas/gfortran. OSX is set up. Windows: set up the MINGW Blas libs on your path.)
    nd4j-netlib-blas
    //(Linux: Install Blas/gfortran. OSX is set up. Windows: set up the MINGW Blas libs on your path.)

where versions can be found on [Maven Central](http://search.maven.org).

For core algorithms, you can simply use:

     <dependency>
         <groupId>org.deeplearning4j</groupId>
         <artifactId>deeplearning4j-core</artifactId>
         <version>${deeplearning4j.version}</version>
     </dependency>
     
For Natural-Language Process (NLP):

     <dependency>
         <groupId>org.deeplearning4j</groupId>
         <artifactId>deeplearning4j-nlp</artifactId>
         <version>${deeplearning4j.version}</version>
     </dependency>

For scaleout (Hadoop/Spark):

### Hadoop

      <dependency>
          <groupId>org.deeplearning4j</groupId>
          <artifactId>cdh4</artifactId>
          <version>${deeplearning4j.version}</version>
      </dependency>


### Spark

      <dependency>
          <groupId>org.deeplearning4j</groupId>
          <artifactId>dl4j-spark</artifactId>
          <version>${deeplearning4j.version}</version>
      </dependency>

Install From Source 
==============================

YOU DON'T HAVE TO DO THIS IF YOU'RE JUST USING THE SOFTWARE FROM MAVEN CENTRAL OR THE DOWNLOADS.

1. Download [Maven](http://maven.apache.org/download.cgi) and set it up in your path.
2. Run setup.sh on Unix and setup.bat on Windows