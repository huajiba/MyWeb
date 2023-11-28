<template>
	<!-- 导航条 -->
		<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
			<div class="container">
				<a class="navbar-brand" href="#">
					<img src="./img/icon.png" style="width: 30px;" /> EasyCode
				</a>
				<!-- 折叠按钮 -->
				<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
					<span class="navbar-toggler-icon"></span>
				</button>

				<div class="collapse navbar-collapse" id="navbarSupportedContent">
					<ul class="navbar-nav mr-auto">
						<li class="nav-item active">
							<a class="nav-link" href="#">主页</a>
						</li>
						<li class="nav-item">
							<a class="nav-link" href="#">网站技术</a>
						</li>
						<li class="nav-item dropdown">
							<a class="nav-link dropdown-toggle" href="#" role="button" data-toggle="dropdown" aria-expanded="false">
								大数据技术
							</a>
							<div class="dropdown-menu">
								<a class="dropdown-item" href="#">数据爬虫</a>
								<a class="dropdown-item" href="#">数据分析</a>
								<div class="dropdown-divider"></div>
								<a class="dropdown-item" href="#">数据可视化</a>
							</div>
						</li>
						<li class="nav-item">
							<a class="nav-link">数据库技术</a>
						</li>
					</ul>
					<form class="form-inline my-2 my-lg-0">
						<input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
						<button class="btn btn-outline-primary my-2 my-sm-0" type="submit">搜索</button>
					</form>
					&nbsp;&nbsp;&nbsp;
					<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal" data-whatever="@mdo">登录</button>
				</div>
			</div>
		</nav>
		
		<!--模态框-->
		<div>
			<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
			  <div class="modal-dialog">
			    <div class="modal-content">
			      <div class="modal-header">
			        <h5 class="modal-title" id="exampleModalLabel">登录</h5>
			        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
			          <span aria-hidden="true">&times;</span>
			        </button>
			      </div>
			      <div class="modal-body">
			        <form>
			          <div class="form-group">
			            <label for="recipient-name" class="col-form-label">用户名:</label>
			            <input type="text" class="form-control" id="recipient-name">
			          </div>
			          <div class="form-group">
			            <label for="recipient-name" class="col-form-label">密码:</label>
			            <input type="password" class="form-control" id="recipient-name">
			          </div>
			        </form>
			      </div>
			      <div class="modal-footer">
			        <button type="button" class="btn btn-secondary" data-dismiss="modal">取消</button>
			        <button type="button" class="btn btn-primary">确定</button>
			      </div>
			    </div>
			  </div>
			</div>
		</div>

</template>

<style scoped>
	
</style>