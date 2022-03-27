# Enable testing on a Java Project

### Pre-requisites
1. Jenkins server on T2.Medium instance (use only java version - yum install java-1.8* )
2. Maven setup in jenkins server

### Procedure: 
1. Install below plug-ins
   1. Junit
   2. Warnings next generation
   3. maven integration

1. Create a Maven Project  
   GitHub URL : https://github.com/ravdy/petclinic.git  
   Maven Goals: clean package checkstyle:checkstyle findbugs:findbugs pmd:pmd  
   Post build action : Record compiler warnings & static analysis results 

2. Run you job
