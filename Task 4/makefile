JC=javac
sources = $(wildcard *.java) 
classes = $(sources:.java=.class)

all: myProject

myProgram: $(classes)

clean :
	rm -f *.class

%.class : %.java
	$(JC) $<

jar: $(classes)
	jar -cvfm laba4.jar MANIFEST.mf $(classes) 

run-jar: jar
	java -jar laba4.jar

