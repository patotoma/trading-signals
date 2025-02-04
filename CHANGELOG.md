### 2.4.0 (2021-10-24)

##### Documentation Changes

- Explain `update` & `getResult` ([f2a0e745](https://github.com/bennycode/trading-signals/commit/f2a0e745f5ba4aba7f60d027ec7a7d44019c8478))

##### New Features

- **BBANDS:** Add faster Bollinger Bands implementation based on numbers ([#338](https://github.com/bennycode/trading-signals/pull/338)) ([d262dad4](https://github.com/bennycode/trading-signals/commit/d262dad415644394c5e738503c6885569d12cd3a))
- Add Standard Deviation ([#337](https://github.com/bennycode/trading-signals/pull/337)) ([b89dbcdc](https://github.com/bennycode/trading-signals/commit/b89dbcdccf1df46086f358345bcd0182e4aef0e9))
- **util:** Add faster average implementation based on numbers ([2029f1c3](https://github.com/bennycode/trading-signals/commit/2029f1c3ec72831de9a8578e3e23d0143d167168))
- **SMA:** Add faster SMA implementation based on numbers ([#336](https://github.com/bennycode/trading-signals/pull/336)) ([ea918088](https://github.com/bennycode/trading-signals/commit/ea918088894850b64bde8221581a5587d97c6a3b))

##### Other Changes

- bennycode/trading-signals into main ([c8120128](https://github.com/bennycode/trading-signals/commit/c8120128ac93ff74ea7075aefe183c749b7a92da))

##### Refactors

- **util:** Change faster prefix ([d4894377](https://github.com/bennycode/trading-signals/commit/d4894377832726c94add3b6a5e6364f77f6b9fad))
- **SMA:**
  - Export FasterSMA from SMA directory ([cfe98337](https://github.com/bennycode/trading-signals/commit/cfe983372e1155dfd652b1951705b728de00cc38))
  - Re-use static `getResultFromBatch` method ([89e08a6a](https://github.com/bennycode/trading-signals/commit/89e08a6a9a0cc699951122dca7285c2a2da98402))
- **EMA:** Calculate weight factor only once ([80b368f1](https://github.com/bennycode/trading-signals/commit/80b368f19b030c6823159cc5062d109bae5ce478))

### 2.3.0 (2021-09-05)

##### Documentation Changes

- Specify technical indicator types ([#316](https://github.com/bennycode/trading-signals/pull/316)) ([edff17ef](https://github.com/bennycode/trading-signals/commit/edff17ef6db556565635b0c6e324fc1dde1399ea))
- Add Technical Analysis Library using Pandas ([7cf77846](https://github.com/bennycode/trading-signals/commit/7cf7784610378c2c5e68815d41312d99cefe0330))
- Add Technical Analysis Library using Pandas ([26baa759](https://github.com/bennycode/trading-signals/commit/26baa75960b8d44191df75aacdb0390f4a5d9b1f))

##### New Features

- **STOCH:** Add Stochastic Oscillator ([#314](https://github.com/bennycode/trading-signals/pull/314)) ([6d13ca6a](https://github.com/bennycode/trading-signals/commit/6d13ca6a6702d21cf7837fa9e919759c2da504dd))
- **WSMA:** Add Wilder's Smoothed Moving Average (WSMA) ([#313](https://github.com/bennycode/trading-signals/pull/313)) ([a9a94343](https://github.com/bennycode/trading-signals/commit/a9a943439f66c643adc7a83b2f94a5505d07a7ad))
- **ADX,ATR,RSI:** Add option to use EMA or SMA for smoothing results ([#312](https://github.com/bennycode/trading-signals/pull/312)) ([c75f34e7](https://github.com/bennycode/trading-signals/commit/c75f34e7673d7462e4de1c58d92a8e524593269a))

##### Refactors

- **ADX,ATR,STOCH:** Share high low close type ([e3d677f5](https://github.com/bennycode/trading-signals/commit/e3d677f527c6eaeadbcb2f6626402484ca74b43c))
- **ABANDS,BBANDS:** Reorganize source code files ([300b4413](https://github.com/bennycode/trading-signals/commit/300b441382bf71e5eaf9bcfb5245960ac1c5dc67))

### 2.2.0 (2021-08-29)

##### New Features

- Export `SimpleIndicator` & `Indicator` interface ([2e7e5447](https://github.com/bennycode/trading-signals/commit/2e7e5447125376c93b0a81c2d546b5f1debe1879))

### 2.1.0 (2021-08-28)

##### New Features

- **EMA,DEMA,MACD:** Don't emit values before minimum amount of data is received ([#308](https://github.com/bennycode/trading-signals/pull/308)) ([9074514c](https://github.com/bennycode/trading-signals/commit/9074514ce9d7e40b8d772817255ddff5aed40d0c))

##### Refactors

- Mark overridden functions ([ad94144b](https://github.com/bennycode/trading-signals/commit/ad94144bf5c07fc1a9123cac5eac7a35ac12437b))

#### 2.0.1 (2021-08-28)

##### New Features

- **util:** Export utilities ([bb59af17](https://github.com/bennycode/trading-signals/commit/bb59af17e9443a3b089eb777e7467a1ff31a4465))

##### Bug Fixes

- **SMMA,RSI,ATR,ADX:** Don't cache more prices than necessary to fill the interval ([#307](https://github.com/bennycode/trading-signals/pull/307)) ([2bb0a638](https://github.com/bennycode/trading-signals/commit/2bb0a638e84ea605526d9314f8887609e486f7eb))

## 2.0.0 (2021-08-15)

##### New Features

- **AC,AO,ATR,CG,DEMA,EMA,MOM,ROC,RSI,SMA,SMMA:** Save highest & lowest values for all simple indicators ([#295](https://github.com/bennycode/trading-signals/pull/295)) ([7c6433be](https://github.com/bennycode/trading-signals/commit/7c6433be075994d2b21fb9f02ae462bf257d825e))

#### 1.10.2 (2021-08-12)

##### New Features

- **AC,AO:** Directly return result on update ([1ea3efe4](https://github.com/bennycode/trading-signals/commit/1ea3efe45d29a0fc3ea6c3791127185c85d89e29))

#### 1.10.1 (2021-08-05)

##### Refactors

- **AC,AO:** Expose internal indicators ([71273704](https://github.com/bennycode/trading-signals/commit/71273704fcd878a2a82c3346c9ee5e3a541c0390))

### 1.10.0 (2021-08-05)

##### New Features

- Add Momentum to Accelerator Oscillator ([#290](https://github.com/bennycode/trading-signals/pull/290)) ([ae9bc24e](https://github.com/bennycode/trading-signals/commit/ae9bc24eb318e0bdad7c64c1d54a5ca28e0885c7))
- Add Momentum (MOM) ([#289](https://github.com/bennycode/trading-signals/pull/289)) ([eea7899f](https://github.com/bennycode/trading-signals/commit/eea7899ff9eb78b2b7a70fd068570ff0f0bcc331))
- Add Accelerator Oscillator (AC) ([#288](https://github.com/bennycode/trading-signals/pull/288)) ([2fd93c20](https://github.com/bennycode/trading-signals/commit/2fd93c204454c6051371799ea759fe573b50d9b1))

##### Refactors

- **util:** Export `getAverage` separately ([6f4a1c58](https://github.com/bennycode/trading-signals/commit/6f4a1c58d63d34b51cd41967f75dd8bf416ae962))

### 1.9.0 (2021-08-04)

##### New Features

- Add Awesome Oscillator (AO) ([#287](https://github.com/bennycode/trading-signals/pull/287)) ([2dcba835](https://github.com/bennycode/trading-signals/commit/2dcba835b4f873848cefc034cab3e21348c51046))

### 1.8.0 (2021-07-20)

### 1.7.0 (2021-06-11)

##### New Features

- **ADX:** Return directional indicators (+DI & -DI) ([458466fe](https://github.com/bennycode/trading-signals/commit/458466fe51109c5bd9742e51da6b1bf6abd419e9))

#### 1.6.1 (2021-04-17)

##### Bug Fixes

- **macd:** Ensure MACD histogram compatibility with Tulip Indicators ([#219](https://github.com/bennycode/trading-signals/pull/219)) ([3e27d4e9](https://github.com/bennycode/trading-signals/commit/3e27d4e9caf2f8d4a43851158f57527439ae2f09))

### 1.6.0 (2021-02-16)

##### New Features

- Add Center of Gravity (CG) oscillator ([#185](https://github.com/bennycode/trading-signals/pull/185)) ([f5aa6137](https://github.com/bennycode/trading-signals/commit/f5aa6137b8d2186443c2e4ea9e77661fc9e2b7e8))
- **ADX:** Make interval public ([81351743](https://github.com/bennycode/trading-signals/commit/813517436ed8845769f097ef5ed55af651d84093))

#### 1.5.1 (2021-02-08)

### 1.5.0 (2021-02-08)

##### New Features

- Expose read-only intervals ([f849a8c5](https://github.com/bennycode/trading-signals/commit/f849a8c5c01f1f2c25833b9425040f8b52e2dffd))

### 1.4.0 (2021-02-06)

##### New Features

- Add Acceleration Bands (ABANDS) indicator ([#175](https://github.com/bennycode/trading-signals/pull/175)) ([67d1d881](https://github.com/bennycode/trading-signals/commit/67d1d8813cae2a9d6ea9b92926cc9114cc0d50b4))

### 1.3.0 (2021-01-31)

##### Bug Fixes

- Align MACD results with Tulip Indicators ([#171](https://github.com/bennycode/trading-signals/pull/171)) ([5923be10](https://github.com/bennycode/trading-signals/commit/5923be1078fb2c4964785d36fdf1d26096c19ac6))

#### 1.2.1 (2020-12-09)

##### Bug Fixes

- Check long interval when using moving average crossover with EMA ([#142](https://github.com/bennycode/trading-signals/pull/142)) ([4c218a9e](https://github.com/bennycode/trading-signals/commit/4c218a9e467dca41dd3579ed30ab55bbb2765f6e))

### 1.2.0 (2020-11-05)

##### New Features

- Add option to use EMA for DMA calculation ([#116](https://github.com/bennycode/trading-signals/pull/116)) ([90323796](https://github.com/bennycode/trading-signals/commit/90323796cc94604b6a84b5deb9f620d9e0d4b33b))

#### 1.1.1 (2020-09-06)

### 1.1.0 (2020-09-04)

##### New Features

- Add option to use EMA for RSI calculation ([#70](https://github.com/bennycode/trading-signals/pull/70)) ([33b7b750](https://github.com/bennycode/trading-signals/commit/33b7b750c387926fa551b6ee86fc2fe64b29360e))

#### 1.0.1 (2020-06-15)

## 1.0.0 (2020-06-03)

##### New Features

- Add Average Directional Index (ADX) indicator ([#14](https://github.com/bennycode/trading-signals/pull/14)) ([1a21d531](https://github.com/bennycode/trading-signals/commit/1a21d531519d4a5c61d0eb51ab89651319b412f4))
- Add `isStable` to DMA indicator ([5f1f9dcb](https://github.com/bennycode/trading-signals/commit/5f1f9dcb30f2e4238d54db5f542c8534c9a66294))

### 0.4.0 (2020-06-01)

##### New Features

- Add Average True Range (ATR) indicator ([#13](https://github.com/bennycode/trading-signals/pull/13)) ([e6f88ea8](https://github.com/bennycode/trading-signals/commit/e6f88ea8f3d39d3679b57dff842b4f35c01c9749))

### 0.2.0 (2020-06-01)

### 0.1.0 (2020-05-31)

##### New Features

- Add Moving Average Convergence Divergence (MACD) indicator ([#7](https://github.com/bennycode/trading-signals/pull/7)) ([38a645de](https://github.com/bennycode/trading-signals/commit/38a645de45db1fb2e072c4dfb9df9a124600ef9a))

#### 0.0.5 (2020-05-30)

##### New Features

- Add Rate-of-Change (ROC) indicator ([#4](https://github.com/bennycode/trading-signals/pull/4)) ([f02b5efe](https://github.com/bennycode/trading-signals/commit/f02b5efe061220fa73c1300c6fd88ede4b0e211c))

#### 0.0.4 (2020-05-30)

##### New Features

- Add Relative Strength Index (RSI) ([#3](https://github.com/bennycode/trading-signals/pull/3)) ([f49f897c](https://github.com/bennycode/trading-signals/commit/f49f897cd3ce718b7ab17c4777e8d47d82219c4d))
- Accept input of type number, string & Big ([13aaa996](https://github.com/bennycode/trading-signals/commit/13aaa9965ba51a21d91da055e4e379d900f19dff))

#### 0.0.2 (2020-05-28)

##### Other Changes

- SMA & EMA ([#1](https://github.com/bennycode/trading-signals/pull/1)) ([820842d6](https://github.com/bennycode/trading-signals/commit/820842d62d5bbe20991b0c2742f6f9d7aafff66d))

#### 0.0.1 (2020-05-28)

#### 0.0.2 (2020-05-28)

#### 0.0.1 (2020-05-28)

##### Other Changes

- SMA & EMA ([#1](https://github.com/bennycode/trading-signals/pull/1)) ([820842d6](https://github.com/bennycode/trading-signals/commit/820842d62d5bbe20991b0c2742f6f9d7aafff66d))

#### 0.0.1 (2020-05-28)

##### Other Changes

- SMA & EMA ([#1](https://github.com/bennycode/trading-signals/pull/1)) ([820842d6](https://github.com/bennycode/trading-signals/commit/820842d62d5bbe20991b0c2742f6f9d7aafff66d))
