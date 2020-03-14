# HDFS

Created By: Geunho Lee
Last Edited: Mar 14, 2020 1:03 PM
Tags: HDFS

![HDFS/Untitled.png](HDFS/Untitled.png)

- Scale-up
- Scale-out

![HDFS/Untitled%201.png](HDFS/Untitled%201.png)

- 구글 파일 시스템의 오픈소스화 → HDFS (사용한 언어와 이름만 좀 바뀜)

![HDFS/Untitled%202.png](HDFS/Untitled%202.png)

1. HDFS client API를 통해서 요청하면
2. Namenode에서 location 가져오고
3. Stream API 통해서 타겟 datanode 값들 읽는 방식

### HDFS Client

    hdfs dfs -help
    hdfs dfs -usage <utility_name>

    hdfs dfs -ls -R -h /data/wiki
    hdfs dfs -mkdir /foo/bar
    hdfs dfs -rm deep
    hdfs dfs -touchz file.txt

    hdfs dfs -put <src> <dst>
    hdfs dfs -get <HDFS location> <Local location>

### Namenode Architecture

![HDFS/Untitled%203.png](HDFS/Untitled%203.png)

![HDFS/Untitled%204.png](HDFS/Untitled%204.png)

### File Types

**Test formats**

- csv, tsv, json, xml
- Human readable
- Textual form → Programmable form (Parsing price)
- CSV, TSV → Bad space efficiency, Good speed, Only String
- JSON, XML → Bad space efficiency than CSV, Support various data types

**Binary formats**

![HDFS/Untitled%205.png](HDFS/Untitled%205.png)

- SequenceFile → (Key, Value) 형태

![HDFS/Untitled%206.png](HDFS/Untitled%206.png)

- Columnar File (RCFile, Parquet)

![HDFS/Untitled%207.png](HDFS/Untitled%207.png)

- 많이 쓰는 포맷, 그러나 디테일까지는 지금 알 필요 없음

![HDFS/Untitled%208.png](HDFS/Untitled%208.png)

Conclusion

- 대체로 Binary format 사용하는 것이 빅데이터에선 좋음