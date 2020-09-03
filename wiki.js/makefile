DIR=/Users/pshannon/
DIR=/local/pshannon/github/wiki/wiki.js

dockerRun:
	docker run -d -p 9090:3000 --name wiki --restart unless-stopped \
            -v $(DIR)/config.yml:/wiki/config.yml \
            -v $(DIR)/lc.sqlite:/wiki/database.sqlite \
            requarks/wiki:2

dockerRunTrena:
	docker run -d -p 9090:3000 --name wiki --restart unless-stopped \
            -v $(DIR):/wiki \
            requarks/wiki:2

pull:
	docker pull requarks/wiki:2

