---
layout: post
title: 打造災時不會當機的防災資訊系統
excerpt: 結合防災救災兩階段的資料，建立單一資訊查詢入口；改變系統架構，在平時使用最低資源運作，又可以在災害來臨時期自動擴充，因應大爆量的資料查詢。
image: https://talk.pdis.nat.gov.tw/uploads/default/optimized/1X/0bedf33be909591193c5983b6aae63c83e87653f_1_690x421.png
author: Mark
date: 2017-05-31
---

## 緣起：面對汛期，現有資訊系統的難處？
台灣氣候地形多變，常會發生大大小小的天然災害，如何防災應變，是一個國家安全層級的重要議題。特別是每年汛期，一旦發生災害，政府開設各級應變中心時，各級機關頻繁使用資訊系統即時回報災害情況、民生相關企業與設施也使用資訊系統回報各地災損及復原規劃，是以防救災資訊系統的首要功能，就是作為政府決策及採取適當應變措施的資訊輔助工具。然而另一方面，正如先前PDIS參與協作的[菜價資訊整合平台](https://afabi.pdis.tw)，原先作為決策輔助的資訊系統，在開放政府的理念下，也必須轉換成整合多元資訊、可公開查詢、民眾易用易懂的資訊平台。

尤其防救災關係著民眾的身家財產，如果能讓民眾透過資訊系統查詢災情資料，不僅是滿足人民知的權利，也可以讓民眾採取適當方法避災離災，降低風險損失，同時減輕政府防救災負擔。

防救災資訊系統有其特色，在災害發生，比如說颱風來襲時，隨著災情的發生使用量來到高峰。但是，在沒有災害發生的時候，系統門庭冷落，這有點像台灣的河川「不雨成旱，一雨成澇」，防救災資訊系統也是這樣「荒溪型」的系統吧。

在現有的系統中，防災與救災，分別由「國家災害防救科技中心（NCDR）」以及「內政部消防署」主責。在災害發生前，民眾可以至 NCDR 所提供的「災害情資網」查詢防災資訊。一旦災害發生，進入防災階段，最新消息就會被公布在消防署所提供的「災害情報站」，這樣的不同階段的兩套系統切換，除非熟悉政府運作，對於一般使用者並不友善，無法直覺取得想要的資訊，因而需要邀集跨部會研商系統如何整合。

主責機關與 PDIS 需要共同面對的問題是，如何結合防災救災兩階段的資料，建立單一資訊查詢入口；以及如何改變系統架構，在平時使用最低資源運作，又可以在災害來臨時期自動擴充，因應大爆量的資料查詢。

## 前臺一致、後臺整合
在行政院科技會報辦公室的協助下召開多次會議， PDIS 、消防署與 NCDR與各單位以及廠商務實地研討後，逐漸形成確定的方向，為了達到以單一介面提供資訊的目標，消防署與NCDR雙方系統要逐步整合。整體的整合工作規劃，可分為前端「使用者介面」與後端「資料提供」兩大部分。

前端「使用者介面」，要結合原本兩系統各自的優勢，以滿足不同使用者需求：消防署「災害情報站」簡潔條列式文字呈現，並在畫面上劃分區塊，有利於快速查詢資料；NCDR「災害情資網」互動視覺化介面，利用資料與地圖互動呈現，有利於快速瞭解災害影響範圍。因而未來會從如下圖示左邊的兩個系統介面，合併為圖示右邊的系統介面，而在經費許可的前提下，逐漸朝向比較有利於互動的NCDR使用者介面來整合。

然而，NCDR 原系統設計為了擁有良好的資料查詢彈性，因此消耗較多運算資源，恐怕無法承擔汛期的使用高峰。為了可以在汛期時，特別是災害發生中，提供大量民眾快速查詢，甚至因應瞬間的爆量，NCDR與 PDIS 在技術面討論後，決定變更系統架構。採用預先將各種查詢結果儲存為檔案，以硬碟空間換取運算資源的方式，完成效能精進，同時可在高峰期橫向擴充的系統架構。

在後端「資料提供」部分，因為雙方系統需要的資料格式並不完全相同。除了共同訂定分享格式之外，亦強調需要提供可彈性擴充欄位，以確保在資料交換的過程中，不會因為資料正規化的流程，導致資料內容有所遺失。

<img src="https://talk.pdis.nat.gov.tw/uploads/default/original/1X/e8b7b6cec3f2e9da57247fa7f3db60cedff54df7.png" width="690" height="339">

##運用雲端技術，降低成本、提升可用性
如同前面所說，防救災資訊系統是個「荒溪型」的系統，災害發生時，系統使用量會突然暴增，沒有災害時，系統幾乎沒有人用。針對這樣的特性，固然可以直接增購伺服器來建置，以便於災情發生時，能夠承受大量負載，但就必須購買非常多的運算資源。然而災害並不是常態，如果投入太多固定的資源，平常卻又處於閒置的狀態，這樣的做法並不經濟，在建置上防救災資訊系統長期就是面臨這樣進退兩難的情況。

PDIS認為業界行之有年的雲端運算技術，非常合適處理這樣的情況。正巧中華電信將推出政府專用的 HiCloud 服務（Hicloud Govcloud Region, HGR），先進行測試，預計到 2017 年 9 月正式推出，而 PDIS 剛好是測試使用者之一。因此 PDIS 就與 NCDR 同仁及廠商合作，在HGR上測試「災害情資網-大眾版」，以確保災害來臨時可以使用雲端資源；另一方面，雲端運算技術並不是中華電信所獨有，測試過程也會注意將來不會依賴於任一廠商的雲端服務。

簡言之，HGR 與常見基礎建設即服務（IaaS）供應商提供可以動態擴充或縮減的運算資源，在災害發生時運用大量資源承載民眾查詢，一般時候使用最小資源維持運作。依照實際使用量進行收費（pay-as-you-go）的方式，使得維運成本預計可以大幅降低，卻同時又可以保障高峰期的系統可用性，防救災資訊系統運用這樣的技術，相信可以符合系統需求，又可以達到成本最低，效率最高的目標。

<img src="https://talk.pdis.nat.gov.tw/uploads/default/original/1X/a9ff40741c06c4a94a8c559ecf08d7d4875bcd05.png" width="690" height="326">

## 結語：前後分離、因地制宜採用合適資訊技術

整體而言，防救災資訊系統是PDIS小組繼「菜價公開資訊整合平台」之後，再度與相關部會合作，對一個資料來源多元（跨部會）的大型資訊系統進行整合歸劃，同時依然要達成常態性地提供一般民眾查詢的政策目標。因而除了技術上的要求，也必須從使用者角度強化介面的易用性。但不同於「菜價資訊公開整合平台」，現行防救災資訊系統有消防署及NCDR兩個前端，分別於不同階段提供民眾查詢，所以必須先行整併。

其次，防救災資訊系統如同「菜價公開資訊整合平台」一般，需要整合來自多個不同系統的資料，此時「前後分離」就扮演得非常重要的角色——將前端資料呈現（使用者介面）與後端資料供應，兩者分開設計，如此一來可輕易達成資訊共享與交換，資料呈現介面修正與整合，並可使資訊系統保有彈性，才能因應需求改變進而增減功能。

進一步來說，像防救災資訊系統這樣的「荒溪型」的系統，在政府部門中並不罕見，「[菜價公開資訊整合平台](https://afabi.pdis.tw/)」也是如此，也就是說如果天災造成菜價波動，系統查詢需求也會短期性地大量增加。但菜價查詢只需要讀取靜態資料，所以運用CDN技術（Content Delivery Network，內容傳遞網路）就能解決流量問題。

防救災資訊系統並不相同，不管是氣象、路況還是水電等等資訊，都必須能動態快速寫入更新，才能因應當下防救災的資訊需求。傳統的方式，必須仰賴自身建置大量伺服器，但運用以「租用」代替「購買」的雲端服務模式，不但能解決此一問題，更有效降低建置維護的成本，甚且由於自行購置有可能規劃與需求產生落差，而雲端服務可以彈性擴充，更能確保服務的品質。

PDIS認為以上這些協作經驗，未來也可以協助面臨類似問題的其他政府資訊系統來改善優化。

## 相關連結

* 2017-02-14 與 Rufus Pollock 討論本案 ([英文逐字紀錄](https://sayit.pdis.nat.gov.tw/2017-02-14-open-discussion-with-rufus-pollock))

* 2017-02-14 雲辦 EMIC 廠商會議 ([逐字紀錄](https://sayit.pdis.nat.gov.tw/2017-02-14-%E9%9B%B2%E8%BE%A6emic%E5%BB%A0%E5%95%86%E6%9C%83%E8%AD%B0))

* 2017-03-02 防災系統資訊整合會議 ([逐字紀錄](https://sayit.pdis.nat.gov.tw/2017-03-02-%E9%98%B2%E7%81%BD%E7%B3%BB%E7%B5%B1%E8%B3%87%E8%A8%8A%E6%95%B4%E5%90%88%E6%9C%83%E8%AD%B0))

* 2017-05-23 究心公益科技來訪 ([逐字紀錄](https://sayit.pdis.nat.gov.tw/2017-05-23-%E7%A9%B6%E5%BF%83%E5%85%AC%E7%9B%8A%E7%A7%91%E6%8A%80%E4%BE%86%E8%A8%AA))