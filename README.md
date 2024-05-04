// Define Your Trade Contract Block
TradeContract {
    Market: 'R_100', // Replace with your desired market
    TradeType: 'CALL' if even, 'PUT' if odd,
    ContractType: 'CALL' if even, 'PUT' if odd,
    DefaultCandleInterval: Set as needed,
    RunOnceAtStart: Enabled,
    DefineTradeOptions: Set any additional options (e.g., duration, amount)
}

// Watch and Purchase Your Contract Block
WatchAndPurchase {
    Watch: 'R_100', // Replace with your desired market
    If evenPercentage >= 10.5%, Purchase CALL contract,
    If oddPercentage >= 10.5%, Purchase PUT contract
}
