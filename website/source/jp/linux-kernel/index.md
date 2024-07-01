---
title: Linux Kernel Exploitation
hide_toc: true
---

<div class="balloon_l">
  <div class="faceicon"><img src="img/wolf_normal.png" alt="オオカミくん" ></div>
  <p class="says">
  この章ではカーネル空間におけるExploit手法、いわゆる権限昇格について勉強します。<br>
  WindowsのKernel Exploitでも共通のハードウェアセキュリティ機構や権限昇格の手法が登場するから、この章の知識はLinuxに限らず使えるよ。
  </p>
</div>

- 実行環境とデバッグ方法
  - [カーネルexploitへの導入](introduction/introduction.html)
  - [gdbによるカーネルのデバッグ](introduction/debugging.html)
  - [セキュリティ機構](introduction/security.html)
  - [コンパイルとexploitの転送](introduction/compile-and-transfer.html)
- カーネルエクスプロイトの基礎（LK01: Holstein）
  - [Holsteinモジュールの解析と脆弱性の発火](LK01/welcome-to-holstein.html)
  - [Holstein v1: Stack Overflowの悪用](LK01/stack_overflow.html)
  - [Holstein v2: Heap Overflowの悪用](LK01/heap_overflow.html)
  - [Holstein v3: Use-after-Freeの悪用](LK01/use_after_free.html)
  - [Holstein v4: Race Conditionの悪用](LK01/race_condition.html)
- カーネル空間特有の攻撃
  - [NULL Pointer Dereference (LK02: Angus)](LK02/null_ptr_deref.html)
  - [Double Fetch (LK03: Dexter)](LK03/double_fetch.html)
  - [userfaultfdの利用 (LK04: Fleckvieh)](LK04/uffd.html)
  - [FUSEの利用 (LK04: Fleckvieh)](LK04/fuse.html)
  - [脆弱なmmap実装の悪用 (LK05: Highland) (工事中)](#)
- eBPFとJITコンパイラ (LK06: Brahman)
  - [BPFの導入](LK06/ebpf.html)
  - [検証器とJITコンパイラ](LK06/verifier.html)
  - [eBPFのバグの悪用](LK06/exploit.html)
<!--
- UEFIアプリケーション（LK07: ???）
- TrustZoneとTEE（LK08: ???）
- 付録
  - [buildrootによるカーネルのビルド (工事中)](appendix/buildroot.html)
-->

<div class="column" title="講師プロフィール">
  <div style="overflow: hidden">
    <div style="float: left; margin-right: 1em;" class="faceicon">
      <img src="img/wolf_suyasuya.png" alt="オオカミくん" >
    </div>
    <div style="float: left;">
      <b>オオカミくん</b><br>
      オオカミの群れで権限昇格してリーダーになったという伝説がある。<br>
      動物界ではOS開発の第一人者。基本寝ている。<br>
      好きなもの：牛 / Linux<br>
      苦手なもの：ハイエナ / Windows
    </div>
  </div>
</div>
