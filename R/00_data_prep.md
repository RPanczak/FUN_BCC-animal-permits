---
title: "BCC animal data"
subtitle: "Data preps"
author: "Radoslaw Panczak"
date: "03 April, 2020"
output: 
  html_document: 
    highlight: pygments
    keep_md: yes
    number_sections: yes
    theme: united
    toc: yes
    toc_depth: 4
    toc_float: yes
editor_options: 
  chunk_output_type: console
---

<!-- ------------------------------------------------------------ --> 
<!-- ------------------------------------------------------------ --> 



# Neighbourhood boundaries

## ABS



## QSC




# SEIFA




```
## Rows: 13,713
## Columns: 8
## $ SSC_CODE16 <int> 10001, 10002, 10003, 10004, 10005, 10006, 10007, 10008, 10…
## $ SSC_NAME16 <chr> "Aarons Pass", "Abbotsbury", "Abbotsford (NSW)", "Abercrom…
## $ IRSD       <int> 1, 9, 8, 10, 4, 1, 3, 9, 7, 2, 5, 7, 2, 10, 3, 6, 10, 2, 8…
## $ IRSAD      <int> 1, 9, 10, 9, 4, 1, 2, 9, 6, 1, 4, 8, 2, 10, 2, 7, 9, 2, 7,…
## $ IER        <int> 1, 10, 5, 10, 6, 1, 3, 7, 8, 3, 6, 6, 3, 10, 3, 3, 8, 2, 7…
## $ IEO        <int> 1, 7, 10, 7, 5, 1, 1, 10, 3, 1, 1, 10, 4, 8, 3, 7, 9, 1, 5…
## $ URP        <int> 22, 4253, 5373, 1109, 22, 2473, 2084, 102, 5401, 2337, 348…
## $ caution    <lgl> TRUE, FALSE, FALSE, FALSE, TRUE, FALSE, FALSE, TRUE, FALSE…
```

# Dog cost 




<table>
 <thead>
  <tr>
   <th style="text-align:left;"> dog_breed </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Akita </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Azawakh </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Black Russian Terrier </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Canadian Eskimo Dog </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chow Chow </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Bulldog </td>
  </tr>
  <tr>
   <td style="text-align:left;"> French Bulldog </td>
  </tr>
  <tr>
   <td style="text-align:left;"> French Mastiff </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Shepherd </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hairless Chinese Crested </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Wolfhound </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lowchen </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maltese </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pharaoh Hound </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Rottweiler </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Saint Bernard </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Saluki </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Samoyed </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Mastiff </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Yorkshire Terrier </td>
  </tr>
</tbody>
</table>


# Dog insurance







## Thre major categories

<table class="kable_wrapper">
<tbody>
  <tr>
   <td> 

<table>
 <thead>
  <tr>
   <th style="text-align:left;"> val </th>
   <th style="text-align:left;"> label </th>
   <th style="text-align:right;"> frq </th>
   <th style="text-align:right;"> raw.prc </th>
   <th style="text-align:right;"> valid.prc </th>
   <th style="text-align:right;"> cum.prc </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Above average </td>
   <td style="text-align:left;"> &lt;none&gt; </td>
   <td style="text-align:right;"> 58 </td>
   <td style="text-align:right;"> 10.39 </td>
   <td style="text-align:right;"> 10.39 </td>
   <td style="text-align:right;"> 10.39 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Below average </td>
   <td style="text-align:left;"> &lt;none&gt; </td>
   <td style="text-align:right;"> 457 </td>
   <td style="text-align:right;"> 81.90 </td>
   <td style="text-align:right;"> 81.90 </td>
   <td style="text-align:right;"> 92.29 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Significantly above average </td>
   <td style="text-align:left;"> &lt;none&gt; </td>
   <td style="text-align:right;"> 43 </td>
   <td style="text-align:right;"> 7.71 </td>
   <td style="text-align:right;"> 7.71 </td>
   <td style="text-align:right;"> 100.00 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:left;"> NA </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 0.00 </td>
   <td style="text-align:right;"> NA </td>
   <td style="text-align:right;"> NA </td>
  </tr>
</tbody>
</table>

 </td>
  </tr>
</tbody>
</table>

## Individual breeds

<table>
 <thead>
  <tr>
   <th style="text-align:left;"> dog_breed </th>
   <th style="text-align:left;"> cost_compared_to_other_breeds </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Hygen Hound Cross </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> French Bulldog </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Yorkshire Terrier </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Neopolitan Mastiff </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Grand Basset Griffon Vendeen </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Formosan Mountain Dog </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Newfoundland </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Unknown Dog Breed </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Bulldog Miniature </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Airedale Terrier </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Basset Hound </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bullmastiff </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Great Dane </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Rottweiler </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Weimaraner </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bull Terrier </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Cane Corso </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Bulldog Miniature Cross </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drever </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alaskan Malamute </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Akita </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Bulldog </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bedlington Terrier </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Boxer </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> British Bulldog </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dogue De Bordeaux </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drever Cross </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hygen Hound </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Setter </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Wolfhound </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Mastiff </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Doberman </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Pinscher </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pekingese </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Poodle – Standard </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shar-Pei </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> St Bernard </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Corgi – Cardigan </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Corgi – Pembroke </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wire-Haired Terrier </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Akita Inu </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alaskan Klee Kai </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bernese Mountain Dog </td>
   <td style="text-align:left;"> Significantly above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Corgi – Pembroke Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> British Bulldog Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Corgi </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Weimaraner Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Pinscher Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pinscher </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bull Terrier Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Akita Inu Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Bulldog </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Bulldog Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bedlington Terrier Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bernese Mountain Dog Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Boxer Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chow Chow </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dobermann </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Labrador Retriever </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Mastiff Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Newfoundland Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pekingese Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Poodle – Standard Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> St Bernard Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Corgi – Cardigan Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> King Charles Spaniel </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Polish Lowland Sheepdog Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alaskan Malamute Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Wolfhound Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Rottweiler Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Airedale Terrier Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Akita Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Cocker Spaniel </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Basset Hound Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bullmastiff Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Doberman Pinscher </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dogue De Bordeaux Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Pointer </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> French Bulldog Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Short Haired Pointer Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Great Dane Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Setter Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Labrador </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Doberman Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Poodle </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Old English Sheepdog </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Papillon Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Polish Lowland Sheepdog </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Rhodesian Ridgeback Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Samoyed </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shar-Pei Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Rhodesian Ridgeback </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Cattle Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Greyhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Neopolitan Mastiff Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wire-Haired Terrier Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wolfhound Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Yorkshire Terrier Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Corgi Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fox Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wolfhound </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dalmatian </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pinscher Cross </td>
   <td style="text-align:left;"> Above average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Staffordshire Bull Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Yugoslavian Mountain Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Spitz </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Cobberdog Miniature Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hovawart Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hungarian Kuvasz Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hungarian Puli Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Huntaway Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Red and White Setter Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Greyhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lagotto Rom Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lakeland Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Louisiana Catahoula Leopard Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Manchester Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Mexican Hairless Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Munsterlander – Large Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> New Zealand Huntaway Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norfolk Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norwegian Elk Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norwich Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Nova Scotia Duck Tolling Retriever Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Parson Jack Russell Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Petit Basset Griffon Vendeen Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pharaoh Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Portuguese Water Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schnauzer Giant Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Skye Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Soft Coated Wheaten Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spitz Mittel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Stumpy Tail Cattle Dogs Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swiss Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Mastiff Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Turkish Kangal Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Pointer Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Sheepdog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Spinone Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Japanese Akita Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Japanese Chin Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Komondor Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kuvasz Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Labradoodle Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lurcher Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maltalier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Bull Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund – Smooth Haired Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund – Wire Haired Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund Cross Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund- Long Haired Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Toy Pom Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Munster Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Hunting Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Kelpie Sheepdog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Koolie </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Basset Fauve De Bretagne </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bull Arab Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cane Corso </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dandie Dinmont Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Springer Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Flat Coated Retriever </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Pinscher </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Red and White Setter </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lakeland Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Sarplaninac </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Scottish Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spanador </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Staffordshire Bull Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Sussex Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wire-haired Pointing Griffon Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alaskan Husky </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Patterdale Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Rat Terrior </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cocker Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Cobberdog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Coton De Tulear </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Japanese Akita </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> New Guinea Singing Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Puli Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Saluki Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Sarplaninac Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spanador Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Springer Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swiss Mountain Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swiss Mountain Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alsatian Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Eskimo Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Pit Bull Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Water Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Anatolian Karabosh Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Antartic Husky Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Heeler </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Silky Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd – Laekenois/Groenendael </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Black and Tan Coonhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bloodhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Boerboel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bordeaux Mastiff Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Borzoi Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bouvier Des Flandres </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Brittany Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cairn Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cardigan Corgi Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Central Asian Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Clumber Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Collie (Rough/Smooth) Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund – Long Haired Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund Wire Haired </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dalmatian Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Egyptian Pharoah Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Elkhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Elkhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Mastiff </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Toy terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Estrela </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Field Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Flat Coated Retriever Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Gazelle Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Koolie </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Spitz Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Wire Haired Pointer </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Golden Retriever </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Great Pyrenean </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Greyhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Griffon Brabancon </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Griffon Bruxellois Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Havanese Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hungarian Puli </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Ibizan Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Water Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Sheepdog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Spinone </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kelpie </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Labradoodle </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lurcher </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Malinois Shephard Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Manchester Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund – Smooth Haired </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Maltese Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> New Guinea Singing Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norwegian Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Nova Scotia Duck Tolling Retriever </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Otterhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Papillon </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Parson Jack Russell Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Petit Basset Griffon Vendeen </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pug Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pyrenean Mountain Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Saluki </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schipperke </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schnauzer Giant </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Sealyham Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shetland Sheepdog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shiloh shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Siberian Husky </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spanish Water Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Staghound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Mastiff </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tosa Inu Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Golden Doodle (Groodle) </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund Wire Haired Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Gordon Setter Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kangal Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Afghan Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kerry Blue Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Sealyham Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shiba Inu Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Timber Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Yugoslavian Mountain Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Koolie Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Basset Fauve De Bretagne Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Black and Tan Coonhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Central Asian Ovtcharka </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Collie – Rough </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund – Long Haired </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Deerhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Mastiff Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Pointer Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Field Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Finnish Spitz </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Finnish Spitz Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> HamiltonStovare </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Lagotto Ramgnolo Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Japanese Spitz Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Leonberger </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lhasa Apso </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Louisiana Catahoula Leopard Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lowchen Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Poodle Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Plott Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Plott Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Poodle – Toy </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pug </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Stumpy Tail Cattle Dogs </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swiss Mountain Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tosa Inu </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wire-haired Pointing Griffon </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Wolf/ Wolf Hybrid </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bordeaux Mastiff </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cao De Serra De Aires </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cardigan Corgi </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Egyptian Pharoah Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Setter Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Springer Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Pinscher Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Griffon Brabancon Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> HamiltonStovare Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Water Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Mexican Hairless </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Canaan Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Danish-Swedish Farm Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Prague Ratter </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Smithfield Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spanish Water Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Aberdeen Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Affenpinscher </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alaskan Husky Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Alsatian </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Bulldog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Cocker Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Eskimo </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Foxhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Foxhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Pit Bull Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Staffordshire Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Staffordshire Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> American Water Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Anatolian Karabash </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Anatolian Shepherd Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Anatolian Shepherd Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Antartic Husky </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Cattle Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Cobberdog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Cobberdog Miniature </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Kelpie Sheepdog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Silky Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Basenji </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Basenji Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Beagle </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bearded Collie Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd – Malinois </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd – Malinois Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd – Tervueren </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd – Tervueren Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bichon Frise </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Black Russian Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Black Russian Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bloodhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Blue tick Coonhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Blue tick Coonhound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Boerboel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Border Collie </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Border Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Borzoi </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Boston Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Boston Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bouvier Des Flandres Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Briard </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Briard Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Brittany Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bull Arab </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cane Corso Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cao De Serra De Aires Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cavalier King Charles Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Central Asian Ovtcharka Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Central Asian Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cesky Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cesky Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cheasapeake Bay Retriever </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cheasapeake Bay Retriever Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chinese Crested Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chinese Crested Dog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chow Chow Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Clumber Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cocker Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Collie – Rough Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Collie – Smooth </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Collie – Smooth Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Coton De Tulear Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Curly Coated Retriever Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund – Smooth Haired </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dachshund – Smooth Haired Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dandie Dinmont Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Danish-Swedish Farm Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Deerhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dingo </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dingo Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Doberman Pinscher Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dobermann Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dutch Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dutch Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Setter </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> English Toy terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Estrela Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Finnish Lapphund </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Finnish Lapphund Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fox Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fox Terrier Wire </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fox Terrier Wire Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> French Poodle </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> French Poodle Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Gazelle Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Koolie Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Schnauzer </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Schnauzer Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Short Haired Pointer </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> German Wire Haired Pointer Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Golden Retriever Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Gordon Setter </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Great Pyrenean Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Greek Harehound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Greek Harehound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Greyhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Griffon </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Griffon Bruxellois </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Griffon Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Harrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Harrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Havanese </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hovawart </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hungarian Kuvasz </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hungarian Vizsla </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Hungarian Vizsla Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Huntaway </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Ibizan Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Irish Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Lagotto Ramgnolo </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Italian Pointer </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Japanese Chin </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kangal </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Keeshond </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Keeshond Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kerry Blue </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Komondor </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kuvasz </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Labrador Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Labrador Retriever Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lagotto Rom </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Leonberger Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Malinois Shephard </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maltalier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maltese </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maremma Sheepdog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Bull Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund – Wire Haired </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Dachshund- Long Haired </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Maltese </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Schnauzer </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Schnauzer Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Toy Pom </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Munster </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Munsterlander – Large </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> New Zealand Huntaway </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norfolk Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norwegian Elk Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norwegian Hound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Norwich Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Old English Sheepdog Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Otterhound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pharaoh Hound </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Portuguese Water Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Puli </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pyrenean Mountain Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Samoyed Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schipperke Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schnauzer Standard </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schnauzer Standard Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Scotch Collie </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Scotch Collie Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Scottish Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shiba Inu </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shih Tzu </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shih Tzu Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shiloh shepherd Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Siberian Husky Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Skye Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spitz Mittel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Springer Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Staghound Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Sussex Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swedish Vallhund </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swedish Vallhund Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Swiss Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tenterfield Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Timber Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Turkish Kangal </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Springer Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Welsh Springer Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> West Highland White Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Whippet </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Brazilian Mastiff </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Brazilian Mastiff Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dogo Argentino </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Dogo Argentino Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fila Brasileiro </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fila Brasileiro Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pressa Canario </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pressa Canario Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Aberdeen Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spoodle Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schnoodle Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> King Charles Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bearded Collie </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Greyhound Racing Dog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Whippet Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cavoodle </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Beagle Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Border Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chihuahua </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Japanese Spitz </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lowchen </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Fox Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pomeranian Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Schnoodle </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Shetland Sheepdog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Spoodle </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tenterfield Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Bichon Frise Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Heeler Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Australian Shepherd </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Belgian Shepherd – Laekenois/Groenendael Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Border Collie Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cairn Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Cavalier King Charles Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Chihuahua Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Curly Coated Retriever </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Jack Russell Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Jack Russell Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Kelpie Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Lhasa Apso Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maltese Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Maremma Sheepdog </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Miniature Fox Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Pomeranian </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Soft Coated Wheaten Terrier </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Spaniel </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Tibetan Spaniel Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> West Highland White Terrier Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fox Terrier Smooth </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Fox Terrier Smooth Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Poodle – Toy Cross </td>
   <td style="text-align:left;"> Below average </td>
  </tr>
</tbody>
</table>
