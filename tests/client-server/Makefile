all:
	g++ -o client_server main.cpp test_message.pb.cc -std=c++11 -I../../include -pthread -L/usr/local/lib -I/usr/local -lzmq -lprotobuf
message:
	protoc --cpp_out=. test_message.proto
clean:
	$(RM) *.o *~ client_server