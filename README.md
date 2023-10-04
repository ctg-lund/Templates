# Templates

## Delivery
Note regarding delivery guide: currently replaced manually by copying it over /srv/data/ctgstaff/ctg-delivery-guide-v1.1.pdf
We are rebuilding the delivery process and will probably get the template directly from here in the future!

Use pandoc to convert markdown to pdf, installation guide can be found [here](https://gist.github.com/ilessing/7ff705de0f594510e463146762cef779)

Conversion can then be done with command:
```
pandoc -V colorlinks -V urlcolor=NavyBlue Delivery/src/delivery_guide.md -o Delivery/Publish/delivery_guide.pdf
```
Upload the pdf to lfs:
```
scp <pdf> username@lfs603.srv.lu.se:/srv/data/ctgstaff/
```

## PEP
Portable encapsulated projects (PEPs) are a way of storing biological sampledata along with metadata in a human and machine friendly manner. 

A PEP is used to receive data from customers and is then returned back to the customer along with any additional annotations that might be important.

For the interested see:
http://pep.databio.org/en/latest/
