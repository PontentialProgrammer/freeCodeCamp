---
id: 5e9a093a74c4063ca6f7c161
title: Reading Data Introduction
challengeType: 11
isHidden: true
videoId: cDnt02BcHng
---

## Description
<section id='description'>
</section>

## Tests
<section id='tests'>

```yml
question:
  text: |
    Given a file named `certificates.csv` with these contents:

    ```
    Name$Certificates$Time (in months)
    Tom$8$16
    Kris$2$5
    Ahmad$5$9
    Beau$6$12
    ```

    Fill in the blanks for the missing arguments below:

    ```py
    import csv

    with open(__A__, 'r') as fp:
        reader = csv.reader(fp, delimiter=__B__)
        next(reader)
        for index, values in enumerate(reader):
            name, certs_num, months_num = values
            print(f"{name} earned {__C__} certificates in {months_num} months")
    ```
  
  answers:
    - |
      A: `'certificates.csv'`
      
      B: `'-'` 
      
      C: `values`
    - |
      A: `'certificates.csv'`
      
      B: `'$'`
      
      C: `certs_num`
    - |
    
      A: `'certificates'`
      
      B: `'$'`
      
      C: `certs_num`
  solution: 2
```

</section>

