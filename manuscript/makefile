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
	convert figures/Figure1.png -colorspace CMYK -units PixelsPerInch figures/Figure1.tiff
	convert figures/Figure2.png -colorspace CMYK -units PixelsPerInch figures/Figure2.tiff
	convert figures/Figure3.png -colorspace CMYK -units PixelsPerInch figures/Figure3.tiff
	convert figures/Figure4.png -colorspace CMYK -units PixelsPerInch figures/Figure4.tiff
	convert figures/Figure5.png -colorspace CMYK -units PixelsPerInch figures/Figure5.tiff
	convert figures/Figure6.png -colorspace CMYK -units PixelsPerInch figures/Figure6.tiff
	convert figures/Figure7.png -colorspace CMYK -units PixelsPerInch figures/Figure7.tiff
	convert figures/Figure8.png -colorspace CMYK -units PixelsPerInch figures/Figure8.tiff
	convert figures/Figure9.png -colorspace CMYK -units PixelsPerInch figures/Figure9.tiff

# Show the DPI of each tiff-converted figure
dpi:
	identify -format "%[fx:resolution.x*2.54] DPI\n" figures/Figure*.tiff > figures/figure_dpi.txt

# Remove unused files
clean:
	rm *.aux *.bbl *.blg *.log *.lof *.lot *.synctex.gz *.out
