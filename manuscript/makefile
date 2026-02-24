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
	convert figures/Figure1_1.png -colorspace CMYK -units PixelsPerInch figures/Figure1_1.tiff
	convert figures/Figure2_1.png -colorspace CMYK -units PixelsPerInch figures/Figure2_1.tiff
	convert figures/Figure2_2.png -colorspace CMYK -units PixelsPerInch figures/Figure2_2.tiff
	convert figures/Figure2_3.png -colorspace CMYK -units PixelsPerInch figures/Figure2_3.tiff
	convert figures/Figure2_4.png -colorspace CMYK -units PixelsPerInch figures/Figure2_4.tiff
	convert figures/Figure2_5.png -colorspace CMYK -units PixelsPerInch figures/Figure2_5.tiff
	convert figures/Figure2_6.png -colorspace CMYK -units PixelsPerInch figures/Figure2_6.tiff

# Show the DPI of each tiff-converted figure
dpi:
	identify -format "%[fx:resolution.x*2.54] DPI\n" figures/Figure*.tiff > figures/figure_dpi.txt

# Remove unused files
clean:
	rm *.aux *.bbl *.blg *.log *.lof *.lot *.synctex.gz *.out
