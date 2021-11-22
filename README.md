# hse21_hw3  
# Часть 1  
Ссылка на коллаб - https://colab.research.google.com/drive/19DpE69hyh7oSkcewCBrt-r74ojsGsx43?usp=sharing
# Проверка качества чтений из fastQC: сравнительная статистика из multiQC
![image](https://user-images.githubusercontent.com/60805733/142776373-05b11b52-924e-477f-8e98-42420cdf1f3f.png)  
![image](https://user-images.githubusercontent.com/60805733/142776385-9d5c4216-6283-468f-9622-ac1eb94a5b9c.png)  
![image](https://user-images.githubusercontent.com/60805733/142776392-b85c6c14-fe13-4f48-be6e-edde19a727b2.png)  
![image](https://user-images.githubusercontent.com/60805733/142776399-529eb5f7-c2de-4830-9b3b-dfb4bdf5523c.png)  
![image](https://user-images.githubusercontent.com/60805733/142776411-a7a90224-7d31-4d85-8d1f-66c6afb5d872.png)  
![image](https://user-images.githubusercontent.com/60805733/142776415-668765df-9d25-47c0-8ac1-cab95c8999c5.png)  
![image](https://user-images.githubusercontent.com/60805733/142776424-64035515-e04f-4b67-a028-cbc9a12bd12f.png)  
# Суммарная статистика
![image](https://user-images.githubusercontent.com/60805733/142776458-f388e537-633f-4e17-bf85-0fc809f3e379.png)  
# Количество уникально картированных чтений по каждому образцу:  
![image](https://user-images.githubusercontent.com/60805733/142800576-6f3a3f14-b979-429f-b770-8d1cc56c5281.png)  
# Смотрим статистику HTSeq и узнаем, количество чтений соответствует участкам генома, где не аннотировано ни одного экзона и количество чтений, которые могут принадлежать разным генам  
![image](https://user-images.githubusercontent.com/60805733/142810569-f342aac0-46d7-47c0-9978-24edc16a1799.png)
# С помощью данный, приведенных выше, можно посчитать количество чтений, соответствующих хотя бы одному гену 
![image](https://user-images.githubusercontent.com/60805733/142816386-b3d787a5-7bdc-4744-8ec0-2bfacd4a5886.png)  
# Наглядная статистика по каждому из 6 образцов  
![image](https://user-images.githubusercontent.com/60805733/142847352-2a283267-b805-4aa6-b4f9-dc9e2aeb53ec.png)  
# Объединяем файлы с прочтениями в один - all_counts (столбцы - образцы, при чем c1, c2, c3 - контрольные образцы; r1, r2, r3 - перепрограммированные образцы)  
![image](https://user-images.githubusercontent.com/60805733/142817878-94b29c87-916e-4cea-bcea-0e599d5fef7c.png)

# Часть 2. Анализ с помощью DESeq2  
Ссылка на коллаб - https://colab.research.google.com/drive/1DMjup_hBYMt1yWuY3nqbQEV2HOWfkc7v?usp=sharing
# MA-plot, показывающий Log2FC для генов  
Можно заметить, что большее количество дифференциально экспрессированных генов увеличило свою экспрессию 
![image](https://user-images.githubusercontent.com/60805733/142847394-e503364c-facf-469a-ba19-36e4e3a05c4c.png)  
# Heatmap, показывающий созависимость экспрессии генов из контрольных и репрограммированных образцов  
Можно заметить, что экспрессия генов одинакова в одной группе образцов и отличается между группами  
![image](https://user-images.githubusercontent.com/60805733/142847436-5a8fa829-44ba-4de2-bfc1-6f280e29d661.png)  
# Heatmap для первых 20 наиболее дифференциально экспрессированных генов
![image](https://user-images.githubusercontent.com/60805733/142847475-36ec4b91-452e-46e4-be96-8367fd02fc11.png)  
# Графики со значениями "Normalized counts" в контрольных и перепрограммированных образцах
