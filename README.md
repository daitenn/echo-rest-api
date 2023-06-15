# The Clean Archtecture


![image](https://github.com/daitenn/echo-rest-api/assets/101037787/a20c3750-3688-4e72-ae2d-da5b7740e72d)

# Diagram

![スクリーンショット 2023-06-15 21 58 19](https://github.com/daitenn/echo-rest-api/assets/101037787/2fb6af8d-12a2-4a0d-b38d-072e8ca50382)

- 依存性逆転の法則を用いて、CleanArchtectureの中核に矢印が向かうように実装していることで、例えば現在はPostgreSQLをDBとして扱っていますが、これに仕様変更が加わり、
  MySQLに変更になった場合でもコア部分のロジックを変更することなく、最小限のロジック変更で（今回の場合だと、repository層のロジックの変更）仕様変更に対応できる設計手法をとっています。
