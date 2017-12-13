## reproduce method

data ： DEFAULT.KYLIN_SALES.csv
cube：kylin_sales_cube.json

sql
```
select OPS_REGION,count(1) from KYLIN_SALES group by OPS_REGION;
```

## log
when error comes, I have logged it:
```
   if (comparator.compare(last, fetched) > 0)
   logger.error("comarator:{}, class: {}, last:{}, fetched: {}", comparator.getClass().getName(),                            last.getClass().getName(), last, fetched);
```
                            
                            
2017-12-13 09:47:26,668 ERROR [Query d15d3634-f2a0-4486-8484-dfc62b29a997-76] gtrecord.SortedIteratorMergerWithLimit:142 : comarator:org.apache.kylin.storage.gtrecord.SequentialCubeTupleIterator$1, class: org.apache.kylin.metadata.tuple.Tuple, last:TRANS_ID=null,PART_DT=null,LSTG_FORMAT_NAME=null,LEAF_CATEG_ID=null,LSTG_SITE_ID=null,SLR_SEGMENT_CD=null,PRICE=null,ITEM_COUNT=null,SELLER_ID=null,BUYER_ID=null,OPS_USER_ID=null,OPS_REGION=cn:？？？,_KY_COUNT__=3344,, fetched: TRANS_ID=null,PART_DT=null,LSTG_FORMAT_NAME=null,LEAF_CATEG_ID=null,LSTG_SITE_ID=null,SLR_SEGMENT_CD=null,PRICE=null,ITEM_COUNT=null,SELLER_ID=null,BUYER_ID=null,OPS_USER_ID=null,OPS_REGION=cn:�苏�,_KY_COUNT__=3349,