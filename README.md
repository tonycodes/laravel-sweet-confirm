# Laravel Sweet Confirm
A simple Laravel Blade partial to add Sweet Alert confirmations to your forms. Ideal for when you need to ask you user if they really want to complete the action. (Requires <a href="https://github.com/uxweb/sweet-alert">Sweet Alert</a>).

# Usage
1. Include the partial in your view
<code>@include('partials/scripts/action-confirm.blade.php</code>
2. Add the class confirm to your form and the button for the form
<h2>Example:</h2>

`{!! Form::open(['route' => ['files.delete',$file->id], 'method' => 'get','class'=>'confirm form-horizontal']) !!}`

`<button class="btn btn-danger btn-sm confirm" data-toggle="tooltip" title="Delete">
  Delete
</button>`
