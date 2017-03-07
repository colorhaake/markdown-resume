# 如何用Markdown去產生Resume

## [markdown-resume](https://github.com/there4/markdown-resume)  
依照裡面的指示，下載它編譯好的[phar file](https://github.com/there4/markdown-resume/raw/master/bin/md2resume), 安裝[wkhtmltopdf](https://github.com/pdfkit/pdfkit/wiki/Installing-WKHTMLTOPDF)來產生pdf  
並且輸入下面的指令即可產生相對應的html/pdf file

```
./bin/md2resume html examples/source/sample.md examples/output/
./bin/md2resume pdf examples/source/sample.md examples/output/
```

### 指定你要的template  
`./bin/md2resume html --template blockish examples/source/sample.md examples/output/`

目前template共有[五種](https://github.com/there4/markdown-resume/tree/master/templates) `blockish`, `modern`, `readable`, `swissen`, `unstyled`  

## [davidhampgonsalves/resume](https://github.com/davidhampgonsalves/resume)  
這個tool其實本質上還是用到第一個tool，但是我比較喜歡他的[template](http://www.davidhampgonsalves.com/html/resume.html)，所以我的resume就採用他的tool  
安裝步驟就依照他上面的指示：  
`clone project and npm install`  
`remove the existing core css files in node_modules/markdown-resume/assets/css and move resume.css into that dir.`  
要產生pdf的版本的resume，記得要去安裝[wkhtmltopdf](https://github.com/pdfkit/pdfkit/wiki/Installing-WKHTMLTOPDF)來產生pdf  

如果產生出來的pdf格式怪怪的，可以去安裝舊版的[wkhtmltopdf](http://wkhtmltopdf.org/downloads.html#stable)來產生pdf