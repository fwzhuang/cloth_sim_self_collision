これは[「Computer Graphics Gems JP 2013/2014:コンピュータグラフィックス技術の最前線」](https://www.amazon.co.jp/dp/4862462197)の第九章「自己衝突を含む衣服の有限要素法シミュレーション」の付録ソースコードです。


## ライセンス
+ 全てのコードの著作権は梅谷信行(Nobuyuki Umetani)に帰属します。ソースコードを再配布する場合は必ず著作権を表示して下さい。
+ 研究用途のみに使って下さい。このコードを元に研究をした際の論文などの成果物には本書を引用して下さい。
+  許可なしに商用での使用をしないで下さい。商用での使用を考えている場合は開発者の梅谷(n.umetani@gmail.com)に相談して下さい。


## 免責事項
+ 本コードによって発生した,いかなる損害も一切責任を負いません。


## プロジェクト
+ internal_cloth_eigen: 布の内部物理を解いて布をアニメーションするプロジェクト。連立一次方程式を解くのにEigenライブラリを使用。単純なコードだが低速
+ internal_cloth_sparse: 布の内部物理を解いて布をアニメーションするプロジェクト。連立一次方程式を解くのに独自の疎行列反復ソルバを使用。やや複雑だが高速
+ self_contact_eigen:布の自己接触も含めて布をシミュレーションするプロジェクト。連立一次方程式を解くのにEigenライブラリを使用。単純だが低速</td>
+ self_contact_sparse: 布の自己接触も含めて布をシミュレーションするプロジェクト。連立一次方程式を解くのに独自の疎行列反復ソルバを使用。やや複雑だが高速。


## コンパイル方法
+ Mac用にXCodeのプロジェクトファイル、Windows用にVS2010のプロジェクトファイル、Linux用にMakefileを用意しています。
+ プロジェクト"internal_cloth_eigen"と"self_contact_eigen"をコンパイルするためには
Eigen(http://eigen.tuxfamily.org/)のヘッダファイル群を(./Eigan/)以下に置いて下さい。


## デモ操作
+ 視点の回転：左ボタンドラッグ
+ 衝突オブジェクトの変更：スペースキー
+ アニメーションの計算・停止: 'a'キー


