# Spring Boot Admin Serverのためし

[公式](https://github.com/codecentric/spring-boot-admin/tree/master/spring-boot-admin-samples/spring-boot-admin-sample) がMavenだったのでGradleで。特になんて無く普通に動きそう。

# はまったとこ

* `@EnableAdminServer` の付け忘れ。
    * アノテーション3つ = `@SpringBootApplication` だとゆー思い込みが。
* `de.codecentric.boot.admin` パッケージをうっかりコンポーネントスキャン対象にした。
    * 手を抜いてデフォルトパッケージにしたらだめですね。

