# ESP32-FabGL-MSX1Emulator

[Japanese / [English](#english)]

---

## 概要
ESP32とFabGLライブラリを使用したMSX1エミュレータです（開発中）。

## 構成プロジェクト / Included Projects

1. **MSX Emulator (ESP32)**
   - FabGLベースのMSX本体エミュレータ。

2. **Joystick Converter (STM32)**
   - 一般的なジョイスティックをMSX仕様に変換するためのユニット。


### クレジットと謝辞
- **グラフィック/オーディオエンジン**: [Fabrizio Di Vittorio氏](https://github.com)による FabGL を使用しています。
- **Z80 CPUコア**: Marat Fayzullin氏によるコードをベースに改変して使用しています。
- **VDPセクション**: David Latham氏によるTMS9918Aエミュレーションコアをベースに、Marat Fayzullin氏が調整を加えた実装を改変して使用しています。

### 動作確認済み環境 / ビルド設定
- **ボード**: ESP32 Dev Module
- **ESP32 ボードマネージャ**: v2.0.5 (推奨)
- **使用ライブラリ**: FabGL v1.0.9
- **Arduino IDE 推奨設定**:
  - **PSRAM**: "Enabled" (必須)
  - **Partition Scheme**: "Default 4MB with SPIFFS" 等

### 免責事項・注意事項
- 本ソフトウェア内の各コアのライセンスは、FabGL、および Marat Fayzullin氏 (fMSX License) の各ポリシーに従います。
- 本プロジェクトは開発中であり、不具合や最適化不足なコードが含まれる場合があります。
- 本ソフトウェアの使用によって生じたいかなる損害についても、開発者は一切の責任を負いません。

---

<a name="english"></a>
## English Summary

### Overview
MSX1 Emulator for ESP32 using the FabGL library (Work in Progress).

## 構成プロジェクト / Included Projects

1. **MSX Emulator (ESP32)**
   - MSX main unit emulator based on FabGL.

2. **Joystick Converter (STM32)**
   - A unit to convert standard joysticks for use with MSX.


### Credits & Acknowledgments
- **Graphics/Audio Engine**: [FabGL](https://github.com) by Fabrizio Di Vittorio.
- **Z80 CPU Core**: Based on code by Marat Fayzullin.
- **VDP Section**: Based on TMS9918A core by David Latham, with adjustments by Marat Fayzullin.

### Build Requirements & Settings
- **Board**: ESP32 Dev Module
- **ESP32 Board Manager**: v2.0.5 (Recommended)
- **Required Library**: FabGL v1.0.9
- **Arduino IDE Settings**:
  - **PSRAM**: "Enabled" (Required)
  - **Partition Scheme**: "Default 4MB with SPIFFS" or similar.

### Important Notes & License
- This project adheres to the licenses of FabGL and Marat Fayzullin (fMSX License).
- This is a work in progress; it may contain bugs or unoptimized code.
- The developer is not responsible for any damage caused by using this software.
