all: rlr_annual.zip rlr_monthly.zip met_monthly.zip gslGPChange2014.txt gsl.json
rlr_annual.zip:
	wget -c http://www.psmsl.org/data/obtaining/rlr.annual.data/rlr_annual.zip
rlr_monthly.zip:
	wget -c http://www.psmsl.org/data/obtaining/rlr.monthly.data/rlr_monthly.zip

met_monthly.zip:
	wget -c http://www.psmsl.org/data/obtaining/met.monthly.data/met_monthly.zip

gsl.json: gslGPChange2014.txt
	./csv2json
gslGPChange2014.txt:
	wget -c https://www.psmsl.org/products/reconstructions/gslGPChange2014.txt
