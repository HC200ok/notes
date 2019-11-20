
Vueの$broadcastと$dispatchを再現

Vue1.0では、$broadcastと$dispatchが実装されています、

| componentA
  | componentB
    | componentC

componentA => componentC

componentC => componentA


子コンポーネント（または親コンポーネント）にブロードキャスト（またはディスパッチ）されます。

子コンポーネント（または親コンポーネント）がイベントをリッスンし、trueを返すと、

孫コンポーネントは引き続きイベントをブロードキャスト（または配信）します


ただし、この二つのメソッドはもうVue 2.0で削除されました。
