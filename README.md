# SampleApiWithGoogleSheet

[สร้าง RESTful API บน Google Sheets ใน 5 นาที](https://peerasak.com/post/create-rest-api-in-5-minutes-by-google-sheet/?fbclid=IwAR1LjKsPPHv_RPsYdK0VDkuawa10FaC9k1131chj6vlToomRga0VQKqcTUU)

[Gexpress](https://github.com/coderofsalvation/Gexpress)

[Gexpress-middleware-RESTsheet](https://github.com/coderofsalvation/Gexpress-middleware-RESTsheet)

### Google Apps Script ###
var app = new Gexpress.App()
var sheet = SpreadsheetApp.openById('ใส่ SHEET ID ของคุณ')
var product = GexpressTamotsu.middleware('/products', {sheet:sheet,tab:'products'})

app.use(product);

function doGet(e) { return app.doGet(e); }
function doPost(e) { return app.doPost(e); }
