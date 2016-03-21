SRC := "draft"
SRCXML := $(SRC).xml

all:    text_and_html

text_and_html:  $(SRCXML)
	xml2rfc --html --text $(SRCXML)

text:   $(SRCXML)
	xml2rfc --text $(SRCXML)

html:   $(SRCXML)
	xml2rfc --html $(SRCXML)

# Pull and update this repository.
update:
	git pull -v -u origin master

push:
	git push -v origin master:master

.PHONY:	$(SRCXML)
