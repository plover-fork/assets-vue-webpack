# assets-vue-webpack




// 编译时生效的插件
if (process.env.PLOVER_ASSETS_BUILD) {
  const webpack = require('webpack');
  module.exports.plugins = exports.webpack.plugins.concat([
    new webpack.optimize.UglifyJsPlugin()
  ]);
}
