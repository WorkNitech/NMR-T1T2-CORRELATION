# nmr_t1-t2（元のリポジトリ名）
# NMR-T1T2-CORRELATION
NMRのT1-T2相関測定に関するプロジェクト
## Overview
このリポジトリは、NMR（核磁気共鳴）のT1-T2相関測定を行うためのプログラムの開発に関するプロジェクトである。T1測定（Inversion Recovery法）とT2測定（CPMG法）のプログラムを組み合わせて、T1-T2相関測定を実現する。
このプログラムは、Brukerの装置に対応したExpspell言語で実装される。

## Components
- **T1 Measurement (Inversion Recovery)**: 縦緩和時間（T1）を測定するためのプログラム。
- **T2 Measurement (CPMG)**: 横緩和時間（T2）を測定するためのプログラム。
- **T1-T2 Correlation Measurement**: T1測定とT2測定の結果を組み合わせて、T1-T2相関を解析するプログラム。
- 
## Usage
このプロジェクトは、Brukerの装置やソフトウェアに依存している。適切な設定やパラメータを用いて、T1-T2相関測定を行います。詳細な手順や使用方法は、各ディレクトリのドキュメントを参照。

## Documentation
- [Design Document](./DesignDocument.md): プロジェクトの設計に関するドキュメント。
- [Issues](https://github.com/WorkNitech/NMR-T1T2-Correlation/issues): プロジェクトの進行状況や課題についての情報。

## Contributing
このプロジェクトへの貢献やフィードバックは、IssueやPull Requestで通知。

## License
このプロジェクトは、適切なライセンスの下で公開されています。詳細は`LICENSE`ファイルを参照。
