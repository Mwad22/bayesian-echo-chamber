all: 12-angry-men-analytics.html

R_OPTS=--no-save --no-restore --no-init-file --no-site-file # vanilla, but with --environ

12-angry-men-analytics.html: 12-angry-men-analytics.Rmd $(wildcard 12-angry-men/*)
	R ${R_OPTS} -e "rmarkdown::render('12-angry-men-analytics.Rmd')"

081314-scotus.html: 081314-scotus.Rmd $(wildcard 08-1314/*)
	R ${R_OPTS} -e "rmarkdown::render('081314-scotus.Rmd')"
clean:
	rm -rf 12-angry-men-analytics.html *.Rhistory *.RData