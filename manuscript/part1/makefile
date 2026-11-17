help:
	@echo "Available makes:"
	@echo "figs - convert figures to TIF/CMYK"
	@echo "dpi - show the DPI of each tiff-converted figure"
	@echo "clean - remove unused files"

all:
	make figs
	make dpi
	make clean

# Convert and rename figures
figs:
	convert Figure1_1.png -colorspace CMYK -units PixelsPerInch Figure1_1.tiff

# Show the DPI of each tiff-converted figure
dpi:
	identify -format "%[fx:resolution.x*2.54] DPI\n" Figure*.tiff > figure_dpi.txt

# Remove unused files
clean:
	rm *.aux *.bbl *.blg *.log *.lof *.lot *.synctex.gz *.out
