# PlacesProject

## Purpose Of This Project

- 自分の家にあるものすべてを整理してどこに何があるかシステムを通じて把握できるようにする
- 不用品はシステムを通じて売却することができる
- ほかの利用者と不用品の物々交換や売買ができる

## Business Logic

- Add Places
- Update Places
- Delete Places
- List Places
- Add Area Into Places
- Update Area Details
- Delete Area
- Add Section Into Places
- Add Stuff
- Delete Stuff
- Update Stuff Details
- Export Stuff
- Request Stuff
- Sell Stuff


## Class And Variables

### Places
- name
- description
- address
- owner
- created
- delete_flg

### Area
- name
- place_id(one to many)
- description
- owner
- created
- delete_flg

### Section
- name
- area_id(one to many)
- description
- owner
- created
- delete_flg

### Stuff
- name
- section_id(one to many)
- description
- owner
- created
- delete_flg
- public_flg

### DBManager
- save
- update
- delete
- list

## Test Cases

### LoginView

### HomeView

### ListView


### Places
- Placesの登録に成功すること
- Placesの名称が空白の場合
- Placesの説明が空白の場合

### Area
- Areaの登録に成功すること
- Areaの名称が空白の場合
- Areaの説明が空白の場合

### Section
- Sectionの登録に成功すること
- Sectionの名称が空白の場合
- Sectionの説明が空白の場合

### Stuff
- Placesの登録に成功すること
- Placesの名称が空白の場合
- Placesの説明が空白の場合

### DBManager
- レコードが登録できていること
- レコードが更新できていること
- レコードの一覧が取得できること