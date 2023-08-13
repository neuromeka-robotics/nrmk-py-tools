# 뉴로메카 엔지니어를 위한 Python tools 집합

## 설치
* 사용할 위치에 git 코드 복사

* 의존 패키지 설치
```bash
pip3 install numpy scipy PyYAML matplotlib
```

## 사용
### device.py
- machine(): 현재 시스템 아키텍쳐 리턴
- get_ip_address(): 현재 시스템 IP 주소 리턴

### file_io.py
- save_json(filepath, data), load_json(filepath): json 파일 읽고 쓰기
- save_yaml(filepath, ymlDict), load_yaml(filepath): yaml 파일 읽고 쓰기
- save_text(filepath, data), load_text(filepath): 텍스트 파일 읽고 쓰기
- save_pickle(filepath, obj), load_pickle(filepath): 피클 파일 읽고 쓰기
- create_dir(dir), delete_dir(dir), delete_file(path): 폴더 및 경로 만들고 지우기 
- get_memory_usage_gb() 현재 메모리 사용량 확인

### math_tools.py
- 회전 행렬 및 변환 행렬 연산: ```scripts``` 예제 참조
- T2cmd(Tbe), cmd2T(Tbe_cmd): 변환 행렬과 Indy Task command 간 변환 