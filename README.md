### Ноутбук, визуализирущий NDVI (Normalized Difference Vegetation Index - нормализованный относительный индекс растительности) выбранного участка с помощью открытых данных спутниковой съемки семейства Sentinel-2 

##### _Цель проекта_: получение визуализации вегетационных индексов по формуле NDVI с использованием данных Sentinel-2 с 4 и 8 каналов 

![image](https://user-images.githubusercontent.com/69538737/168348003-e7dd6e21-c330-4469-8a05-173af94cafce.png)

где,
NIR - отражение в ближней инфракрасной области спектра;
RED - отражение в красной области спектра

Расчет NDVI базируется на двух наиболее стабильных (не зависящих от прочих факторов) участках спектральной кривой отражения сосудистых растений. В красной области спектра (0,6-0,7 мкм - B04) лежит максимум поглощения солнечной радиации хлорофиллом высших сосудистых растений, а в инфракрасной области (0,7-1,0 мкм - B08) находится область максимального отражения клеточных структур листа. То есть высокая фотосинтетическая активность (связанная, как правило, с густой растительностью) ведет к меньшему отражению в красной области спектра и большему в инфракрасной. Отношение этих показателей друг к другу позволяет четко отделять и анализировать растительные от прочих природных объектов.

##### Выбранная территория отражена на карте OSM с помощью библиотеки folio и предварительно подготовленного полигона:

![image](https://user-images.githubusercontent.com/69538737/168350942-8bbfd1ae-01dc-40bc-8512-44095bc874b0.png)

##### Результат: растровый снимок одного из выбранных полей в колеровке по шкале NDVI, который показывает дифференциацию значений индекса и выделяет зоны пониженной фотосинтетической активности растений; различия могут быть связаны с типом вспашки, типом засеянной культуры, особенностями рельефа и тп.. 

![image](https://user-images.githubusercontent.com/69538737/168374744-385e8eec-b72b-42e2-9381-465bbfcd5f81.png)



##### А также временной ряд индекса, из которого следует, что наиболее активным периодом развития растений является конец июля.

![image](https://user-images.githubusercontent.com/69538737/168377844-e780dfec-b203-4bc0-8f28-b57b959147d5.png)
  
