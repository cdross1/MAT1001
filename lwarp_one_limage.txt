pdfseparate -f %1 -l %1 %4_html.pdf mat1001-images\lateximagetemp-%%d.pdf
pdfcrop --hires --margins "0 1 0 0" mat1001-images\lateximagetemp-%1.pdf mat1001-images\%3.pdf
pdftocairo -svg -noshrink mat1001-images\%3.pdf mat1001-images\%3.svg
del mat1001-images\%3.pdf
del mat1001-images\lateximagetemp-%1.pdf
exit
