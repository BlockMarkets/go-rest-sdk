# \DefaultApi

All URIs are relative to *https://api.blockmarkets.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BenchmarkRate**](DefaultApi.md#BenchmarkRate) | **Get** /v1/rates/benchmark/{symbol} | Returns the latest available benchmark rates for a specific asset.
[**BenchmarkRateHistory**](DefaultApi.md#BenchmarkRateHistory) | **Get** /v1/rates/benchmark/{symbol}/history | Returns historical benchmark rates for an asset. Requires premium subscription.
[**ListAssetMarkets**](DefaultApi.md#ListAssetMarkets) | **Get** /v1/assets/{symbol} | Returns a list of all markets (base and quote) for a specific asset.
[**ListAssets**](DefaultApi.md#ListAssets) | **Get** /v1/assets | Returns a list of supported assets.
[**ListBenchmarkRates**](DefaultApi.md#ListBenchmarkRates) | **Get** /v1/rates/benchmark | Returns a list of supported USD benchmark rates.
[**ListExchangeMarkets**](DefaultApi.md#ListExchangeMarkets) | **Get** /v1/exchanges/{exchange} | Returns a list of markets for a specific exchange.
[**ListExchanges**](DefaultApi.md#ListExchanges) | **Get** /v1/exchanges | Returns a list of supported exchanges.
[**ListMarkets**](DefaultApi.md#ListMarkets) | **Get** /v1/markets | Returns a list of supported markets.
[**ListPairMarkets**](DefaultApi.md#ListPairMarkets) | **Get** /v1/pairs/{pair} | Returns a list of markets for a specific asset pair.
[**ListPairs**](DefaultApi.md#ListPairs) | **Get** /v1/pairs | Returns a list of supported asset pairs.
[**ListSpotRates**](DefaultApi.md#ListSpotRates) | **Get** /v1/rates/spot | Returns a list of supported USD spot rates.
[**MarketBook**](DefaultApi.md#MarketBook) | **Get** /v1/markets/{exchange}/{pair}/book | Returns the top 50 bids and asks from the current order book for a market pair. Requires premium subscription.
[**MarketOHLCV**](DefaultApi.md#MarketOHLCV) | **Get** /v1/markets/{exchange}/{pair}/ohlcv | Returns OHLCV history for a market pair.
[**MarketTicker**](DefaultApi.md#MarketTicker) | **Get** /v1/markets/{exchange}/{pair} | Returns the latest ticker for a market pair.
[**MarketTrades**](DefaultApi.md#MarketTrades) | **Get** /v1/markets/{exchange}/{pair}/trades | Returns trades for a market pair. Requires premium subscription.
[**SpotRate**](DefaultApi.md#SpotRate) | **Get** /v1/rates/spot/{symbol} | Returns the last USD spot rate for an asset.
[**SpotRateHistory**](DefaultApi.md#SpotRateHistory) | **Get** /v1/rates/spot/{symbol}/history | Returns historical spot rates for an asset. Requires premium subscription.
[**SpotRateOHLCV**](DefaultApi.md#SpotRateOHLCV) | **Get** /v1/rates/spot/{symbol}/ohlcv | Returns the OHLCV history for a spot rate.


# **BenchmarkRate**
> Empty BenchmarkRate(ctx, symbol)
Returns the latest available benchmark rates for a specific asset.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **symbol** | **string**| The asset symbol (see /assets) | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **BenchmarkRateHistory**
> Empty BenchmarkRateHistory(ctx, symbol, optional)
Returns historical benchmark rates for an asset. Requires premium subscription.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **symbol** | **string**| The asset symbol (see /assets) | 
 **optional** | ***BenchmarkRateHistoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BenchmarkRateHistoryOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **close** | **optional.String**| The closing time. Options - 4pm-gmt-close, 4pm-est-close, 0-utc-close | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListAssetMarkets**
> Empty ListAssetMarkets(ctx, symbol)
Returns a list of all markets (base and quote) for a specific asset.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **symbol** | **string**| The asset symbol (see /assets) | 

### Return type

[**Empty**](Empty.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListAssets**
> Empty ListAssets(ctx, )
Returns a list of supported assets.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListBenchmarkRates**
> Empty ListBenchmarkRates(ctx, )
Returns a list of supported USD benchmark rates.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListExchangeMarkets**
> Empty ListExchangeMarkets(ctx, exchange)
Returns a list of markets for a specific exchange.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | **string**| The 4-char exchange code (see /exchanges) | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListExchanges**
> Empty ListExchanges(ctx, )
Returns a list of supported exchanges.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListMarkets**
> Empty ListMarkets(ctx, )
Returns a list of supported markets.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListPairMarkets**
> Empty ListPairMarkets(ctx, pair)
Returns a list of markets for a specific asset pair.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **pair** | **string**| The asset pair (see /pairs) | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListPairs**
> Empty ListPairs(ctx, )
Returns a list of supported asset pairs.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListSpotRates**
> Empty ListSpotRates(ctx, )
Returns a list of supported USD spot rates.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MarketBook**
> Empty MarketBook(ctx, exchange, pair)
Returns the top 50 bids and asks from the current order book for a market pair. Requires premium subscription.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | **string**| The 4-char exchange code (see /exchanges) | 
  **pair** | **string**| The asset pair (see /pairs) | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MarketOHLCV**
> Empty MarketOHLCV(ctx, exchange, pair, optional)
Returns OHLCV history for a market pair.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | **string**| The 4-char exchange code (see /exchanges) | 
  **pair** | **string**| The asset pair (see /pairs) | 
 **optional** | ***MarketOHLCVOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MarketOHLCVOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **optional.Int32**| Number of records to retrieve (default&#x3D;100, max&#x3D;1000) | 
 **interval** | **optional.Int32**| Interval period in minutes. Supported - 1,3,5,15,30,60,1440 (default&#x3D;1440) | 
 **start** | **optional.String**| Start datetime in ISO 8601 | 
 **end** | **optional.String**| End datetime in ISO 8601 | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MarketTicker**
> Empty MarketTicker(ctx, exchange, pair)
Returns the latest ticker for a market pair.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | **string**| The 4-char exchange code (see /exchanges) | 
  **pair** | **string**| The asset pair (see /pairs) | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **MarketTrades**
> Empty MarketTrades(ctx, exchange, pair, optional)
Returns trades for a market pair. Requires premium subscription.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **exchange** | **string**| The 4-char exchange code (see /exchanges) | 
  **pair** | **string**| The asset pair (see /pairs) | 
 **optional** | ***MarketTradesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MarketTradesOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **optional.Int32**| Number of records to retrieve (default&#x3D;100, max&#x3D;1000) | 
 **start** | **optional.String**| Start datetime in ISO 8601 | 
 **end** | **optional.String**| End datetime in ISO 8601 | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpotRate**
> Empty SpotRate(ctx, symbol)
Returns the last USD spot rate for an asset.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **symbol** | **string**| The asset symbol (see /assets) | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpotRateHistory**
> Empty SpotRateHistory(ctx, symbol, optional)
Returns historical spot rates for an asset. Requires premium subscription.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **symbol** | **string**| The asset symbol (see /assets) | 
 **optional** | ***SpotRateHistoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpotRateHistoryOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **optional.Int32**| Number of records to retrieve (default&#x3D;100, max&#x3D;1000) | 
 **start** | **optional.String**| Start datetime in ISO 8601 | 
 **end** | **optional.String**| End datetime in ISO 8601 | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpotRateOHLCV**
> Empty SpotRateOHLCV(ctx, symbol, optional)
Returns the OHLCV history for a spot rate.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **symbol** | **string**| The asset symbol (see /assets) | 
 **optional** | ***SpotRateOHLCVOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpotRateOHLCVOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **optional.Int32**| Number of records to retrieve (default&#x3D;100, max&#x3D;1000) | 
 **interval** | **optional.Int32**| Interval period in minutes. Supported -  1,3,5,15,30,60,1440 (default&#x3D;1440) | 
 **start** | **optional.String**| Start datetime in ISO 8601 | 
 **end** | **optional.String**| End datetime in ISO 8601 | 

### Return type

[**Empty**](Empty.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

