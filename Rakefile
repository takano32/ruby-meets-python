

task default: 'test'

task 'test' => ['hello.so']do
  sh 'ruby -r./hello -e ""'
end


task 'hello.so' => 'hello.pyx' do
  sh 'python setup.py build_ext --inplace'
end


