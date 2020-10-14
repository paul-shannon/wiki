DIR=/Users/paul/github/wiki/wiki.js
#DIR=/local/pshannon/github/wiki/wiki.js

lc:
	docker run -d -p 9091:3000 --name wiki_lc --restart unless-stopped \
            -v $(DIR)/config.yml:/wiki/config.yml \
            -v $(DIR)/lc.sqlite:/wiki/database.sqlite \
            requarks/wiki:2

dockerRunTrena:
	docker run -d -p 9090:3000 --name wiki --restart unless-stopped \
            -v $(DIR):/wiki \
            requarks/wiki:2

pull:
	docker pull requarks/wiki:2



erythro:
	docker run -d -p 9093:3000 --name wiki_erythro_2 --restart unless-stopped \
            -v $(DIR)/erythropoiesis.yml:/wiki/config.yml \
            -v $(DIR)/erythropoiesis.sqlite:/wiki/erythropoiesis.sqlite \
            requarks/wiki:2
