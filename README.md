https://maven.apache.org/plugins-archives/maven-archetype-plugin-1.0-alpha-7/examples/webapp.html
でpom.xml生成

web.xml でバージョンを3.1に上げる

Eclipseで正しく読み込めないので以下を設定
- プロパティのfacetで画面右のタブ Runtimesを開き WildFly10.0 Runtime にチェックを入れる
- Dynamic Web Module のバージョンを 3.1 に更新
- このとき保存できなければ、一旦 Dynamic Web Module のチェックを外し Apply, その後チェックをつけて保存しなおせばOK

maven-war-plugin で webappDirectory を明示しておかないと、Eclipseに初回importした時にエラーになる.
(本来なら無くても良いはずなのだが)
http://stackoverflow.com/a/40893500/4506703


