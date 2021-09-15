# Counting-and-Visualizing-CRAN-Downloads-packageRank-with-Caveats

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.


packageRank is an R package that helps put package download counts into context. It does so via two functions. The first, cranDownloads(), extends cranlogs::cran_downloads() by adding a plot() method and a more user-friendly interface. The second, packageRank(), uses rank percentiles, a nonparametric statistic that tells you the percentage of packages with fewer downloads, to help you see how your package is doing compared to all other CRAN packages.

In this post, I’ll do two things. First, I’ll give an overview of the package’s core features and functions. Second, I’ll discuss a systematic positive bias that inflates download counts.

# CRAN
install.packages("packageRank")

library(packageRank)
library(ggplot2)

