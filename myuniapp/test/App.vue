<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style lang="scss">
	/*每个页面公共css */
	
* {
  font-family: '微软雅黑';
}
/*公用样式*/

.flex {
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
}

.flex-column {
  flex-direction: column;
  -webkit-flex-direction: column;
}

.flex-row {
  flex-direction: row;
  -webkit-flex-direction: row;
}

.flex-space {
  justify-content: space-between;
  -webkit-justify-content: space-between;
}

.flex-start {
  justify-content: flex-start;
  -webkit-justify-content: flex-start;
}

.flex-around {
  align-content: space-around;
  -webkit-align-content: space-around;
}

.flex-end {
  justify-content: flex-end;
  -webkit-justify-content: flex-end;
}

.flex-end-align {
  align-items: flex-end;
  -webkit-align-items: flex-end;
}

.flex-start-align {
  align-items: flex-start;
  -webkit-align-items: flex-start;
}

.flex-bottom {
  align-items: flex-end;
  -webkit-align-items: flex-end;
}

.flex-center {
  justify-content: center;
  -webkit-justify-content: center;
  align-items: center;
  -webkit-align-items: center;
}

.flex-centers {
  -webkit-align-items: center;
  align-items: center;
  -webkit-align-content: center;
  align-content: center;
}

.flex-centersss {
  justify-content: center;
  -webkit-justify-content: center;
}

.flex-centerss {
  -webkit-align-items: center;
  align-items: center;
}

.flex-wrap {
  -webkit-flex-wrap: wrap;
  flex-wrap: wrap;
}

.text-wrap {
  word-wrap: break-word;
  word-break: break-all;
}

.text-hiddle {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  display: inline-block;
}

.text-center {
  text-align: center;
}

.flex-box {
  -webkit-box-flex: 1;
  -ms-flex: 1;
  flex: 1;
}

.flex-strech {
  align-items: stretch;
}

/*超出两行隐藏  */

.flex-hiddens {
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 2;
}

</style>
