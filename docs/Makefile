.PHONY: all clean include

EDITOR ?= gvim
all: md
md: md2html.jar
	java -jar md2html.jar -i . -o docs
watch: md2html.jar
	java -jar md2html.jar -w -i . -o docs 
md2html.jar:
	curl http://whudoc.qiniudn.com/java/md2html/md2html.jar > md2html.jar
clean:
	rm -rf docs/*
e: edit
edit:	
	gvim README.md
