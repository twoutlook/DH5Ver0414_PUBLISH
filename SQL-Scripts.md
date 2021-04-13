# SQL Scripts

## 這是給 C030 使用, 如果沒有這支 sp, 目前畫面看不到預期效果,也沒有報錯。 

```
CREATE OR ALTER PROCEDURE [dbo].[sp_C030] @PIC_NO nvarchar(30)
AS
select distinct a.* from  PIC_DTL a
join LOC_DTL b on(a.SU_ID = b.SU_ID
            and a.SKU_NO = b.SKU_NO
            and a.BATCH_NO = b.BATCH_NO
            and a.COUNT_UNIT = b.GTIN_UNIT)
where a.PIC_NO = @PIC_NO
order by a.PIC_LINE
```
