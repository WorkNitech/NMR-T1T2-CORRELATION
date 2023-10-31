# T1-T2 Correlation Measurement Program Design Document

## 1. Introduction
このドキュメントでは、NMRのT1-T2相関測定を行うためのプログラムの設計について説明します。T1測定（Inversion Recovery法）とT2測定（CPMG法）を組み合わせて、T1-T2相関測定を行います。

## 2. Overview
T1-T2相関測定は、T1測定とT2測定を順番に実行し、その結果を組み合わせて解析するプロセスです。本プログラムは、Brukerの装置に対応したExpspell言語で実装されます。

## 3. Components

### 3.1 T1 Measurement (Inversion Recovery)
#### 3.1.1 Purpose
T1測定は、縦緩和時間（T1）を測定するためのプロセスです。これにより、核スピンが基準状態に戻る時間を測定します。

#### 3.1.2 Parameters and Procedure
- `rd`: リラクセーションディレイ（例: 1000 ms）
- その他、T1測定に関連するパラメータと手順

### 3.2 T2 Measurement (CPMG)
#### 3.2.1 Purpose
T2測定は、横緩和時間（T2）を測定するためのプロセスです。これにより、核スピンの緩和過程を測定します。

#### 3.2.2 Parameters and Procedure
- `te`: エコータイム（例: 10 ms）
- `ne`: エコーの数（例: 32）
- その他、T2測定に関連するパラメータと手順

### 3.3 T1-T2 Correlation Measurement
#### 3.3.1 Purpose
T1-T2相関測定は、T1測定とT2測定の結果を組み合わせて、物質の動的性質を解析するためのプロセスです。

#### 3.3.2 Procedure
- T1測定とT2測定を順番に実行する。
- T1測定とT2測定の結果を組み合わせて、T1-T2相関を解析する。

## 4. Implementation
プログラムは、Expspell言語を使用して実装されます。T1測定のプログラムとT2測定のプログラムを適切に組み合わせて、T1-T2相関測定のプログラムを構築します。

## 5. Testing and Optimization
プログラムは、Brukerの装置でテストされ、必要に応じてパラメータの調整や最適化が行われます。
