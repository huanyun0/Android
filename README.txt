# Android
1
AsyncTask,是android提供的轻量级的异步类,可以直接继承AsyncTask,在类中实现异步操作,并提供接口反馈当前异步执行的程度(可以通过接口实现UI进度更新),最后反馈执行的结果给UI主线程.

AsyncTask定义了三种泛型类型 Params，Progress和Result。

Params 启动任务执行的输入参数，比如HTTP请求的URL。
Progress 后台任务执行的完成的百分比。
Result 后台执行任务最终返回的结果，比如byte[],String。
在AsyncTask中需要注意的几个方法：

onPreExecute()   当任务执行之前开始调用此方法，比如可以在这里将进度对话框显示出来。
doInBackground(Params…) 在后台执行，主要是完成耗时的操作。因为此方法在后台线程执行，所以不能再次更新UI。在执行过程中可以通过调用publicProgress(Progress…)来更新任务的进度。
onPostExecute(Result)  当doInBackground(Params…)方法执行完成之后执行该方法， 此方法在主线程执行,在这里面可以使用在doInBackground返回的结果进行更新UI。
onProgressUpdate(Progress…)   更新进度条加载的进度， 此方法在主线程中执行，可直接进行UI更新。
除此之外，使用过程中还要注意几点：1.AsyncTak实例化以及execute的调用必须要在主线程中完成；2.不能手动调用上面提到的几个方法；3.task不能执行多次，只能执行一次，否则容易出现异常。

2
AsyncTask,是android提供的轻量级的异步类,可以直接继承AsyncTask,在类中实现异步操作,并提供接口反馈当前异步执行的程度(可以通过接口实现UI进度更新),最后反馈执行的结果给UI主线程.

AsyncTask定义了三种泛型类型 Params，Progress和Result。

Params 启动任务执行的输入参数，比如HTTP请求的URL。
Progress 后台任务执行的完成的百分比。
Result 后台执行任务最终返回的结果，比如byte[],String。
在AsyncTask中需要注意的几个方法：

onPreExecute()   当任务执行之前开始调用此方法，比如可以在这里将进度对话框显示出来。
doInBackground(Params…) 在后台执行，主要是完成耗时的操作。因为此方法在后台线程执行，所以不能再次更新UI。在执行过程中可以通过调用publicProgress(Progress…)来更新任务的进度。
onPostExecute(Result)  当doInBackground(Params…)方法执行完成之后执行该方法， 此方法在主线程执行,在这里面可以使用在doInBackground返回的结果进行更新UI。
onProgressUpdate(Progress…)   更新进度条加载的进度， 此方法在主线程中执行，可直接进行UI更新。
除此之外，使用过程中还要注意几点：1.AsyncTak实例化以及execute的调用必须要在主线程中完成；2.不能手动调用上面提到的几个方法；3.task不能执行多次，只能执行一次，否则容易出现异常。

3
AsyncTask,是android提供的轻量级的异步类,可以直接继承AsyncTask,在类中实现异步操作,并提供接口反馈当前异步执行的程度(可以通过接口实现UI进度更新),最后反馈执行的结果给UI主线程.

AsyncTask定义了三种泛型类型 Params，Progress和Result。

Params 启动任务执行的输入参数，比如HTTP请求的URL。
Progress 后台任务执行的完成的百分比。
Result 后台执行任务最终返回的结果，比如byte[],String。
在AsyncTask中需要注意的几个方法：

onPreExecute()   当任务执行之前开始调用此方法，比如可以在这里将进度对话框显示出来。
doInBackground(Params…) 在后台执行，主要是完成耗时的操作。因为此方法在后台线程执行，所以不能再次更新UI。在执行过程中可以通过调用publicProgress(Progress…)来更新任务的进度。
onPostExecute(Result)  当doInBackground(Params…)方法执行完成之后执行该方法， 此方法在主线程执行,在这里面可以使用在doInBackground返回的结果进行更新UI。
onProgressUpdate(Progress…)   更新进度条加载的进度， 此方法在主线程中执行，可直接进行UI更新。
除此之外，使用过程中还要注意几点：1.AsyncTak实例化以及execute的调用必须要在主线程中完成；2.不能手动调用上面提到的几个方法；3.task不能执行多次，只能执行一次，否则容易出现异常。

4
AsyncTask,是android提供的轻量级的异步类,可以直接继承AsyncTask,在类中实现异步操作,并提供接口反馈当前异步执行的程度(可以通过接口实现UI进度更新),最后反馈执行的结果给UI主线程.

AsyncTask定义了三种泛型类型 Params，Progress和Result。

Params 启动任务执行的输入参数，比如HTTP请求的URL。
Progress 后台任务执行的完成的百分比。
Result 后台执行任务最终返回的结果，比如byte[],String。
在AsyncTask中需要注意的几个方法：

onPreExecute()   当任务执行之前开始调用此方法，比如可以在这里将进度对话框显示出来。
doInBackground(Params…) 在后台执行，主要是完成耗时的操作。因为此方法在后台线程执行，所以不能再次更新UI。在执行过程中可以通过调用publicProgress(Progress…)来更新任务的进度。
onPostExecute(Result)  当doInBackground(Params…)方法执行完成之后执行该方法， 此方法在主线程执行,在这里面可以使用在doInBackground返回的结果进行更新UI。
onProgressUpdate(Progress…)   更新进度条加载的进度， 此方法在主线程中执行，可直接进行UI更新。
除此之外，使用过程中还要注意几点：1.AsyncTak实例化以及execute的调用必须要在主线程中完成；2.不能手动调用上面提到的几个方法；3.task不能执行多次，只能执行一次，否则容易出现异常。

5
AsyncTask,是android提供的轻量级的异步类,可以直接继承AsyncTask,在类中实现异步操作,并提供接口反馈当前异步执行的程度(可以通过接口实现UI进度更新),最后反馈执行的结果给UI主线程.

AsyncTask定义了三种泛型类型 Params，Progress和Result。

Params 启动任务执行的输入参数，比如HTTP请求的URL。
Progress 后台任务执行的完成的百分比。
Result 后台执行任务最终返回的结果，比如byte[],String。
在AsyncTask中需要注意的几个方法：

onPreExecute()   当任务执行之前开始调用此方法，比如可以在这里将进度对话框显示出来。
doInBackground(Params…) 在后台执行，主要是完成耗时的操作。因为此方法在后台线程执行，所以不能再次更新UI。在执行过程中可以通过调用publicProgress(Progress…)来更新任务的进度。
onPostExecute(Result)  当doInBackground(Params…)方法执行完成之后执行该方法， 此方法在主线程执行,在这里面可以使用在doInBackground返回的结果进行更新UI。
onProgressUpdate(Progress…)   更新进度条加载的进度， 此方法在主线程中执行，可直接进行UI更新。
除此之外，使用过程中还要注意几点：1.AsyncTak实例化以及execute的调用必须要在主线程中完成；2.不能手动调用上面提到的几个方法；3.task不能执行多次，只能执行一次，否则容易出现异常。
