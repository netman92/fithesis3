LOGS=base.log fi.log sci.log phil.log ped.log fss.log law.log \
	econ.log med.log fsps.log
OUTPUT=fithesis-base.sty fithesis-1[012].clo fithesis-fi.sty \
	fithesis-sci.sty fithesis-phil.sty fithesis-ped.sty \
	fithesis-fss.sty fithesis-law.sty fithesis-econ.sty \
	fithesis-med.sty fithesis-fsps.sty

.PHONY: explode implode all
all: explode
explode: $(LOGS)

%.log: %.ins %.dtx
	xetex $<

implode:
	rm -f $(OUTPUT) $(LOGS)
